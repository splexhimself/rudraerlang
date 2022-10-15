# rudraerlang
-module(diff_pi_tests).
-include_lib("eunit/include/eunit.hrl").
-import(diff_pi, [sum_pi/1]).

sum_pi_test_() ->
    [
        ?_assertEqual(3.0, sum_pi(0)),
        ?_assertEqual(3.1, sum_pi(1)),
        ?_assertEqual(3.14, sum_pi(2)),
        ?_assertEqual(3.141, sum_pi(3)),
        ?_assertEqual(3.1415, sum_pi(4)),
        ?_assertEqual(3.14159, sum_pi(5))
    ].
