# SIR-model-for-covid19-in-Julia
Using SIR-model theory, try to build curve using Julia scientific programming to analyse and pridict how long and how much verse covid19 effect on population.
SIR - susceptible infected removed model for covid19 s(t) = no. of susceptible at time t. s(0) = no. of susceptible at start of epidemic. i(t) and r(t) respectively infected and removed at time t. Remove - The people previously infected but no longer infectious. using principle - New_value = Old_value + gain - losses

By the 'low of mass action' no. of meeting of infected and susceptibles is propotional to S.I. so losses = lambda.S.I.dt (over the time step).

1.s(t+1) = s(t) - lambda.s(t).i(t).dt
2.i(t+1) = i(t) + lambda.s(t).i(t).dt - gamma.i(t).dt
3.r(t+1) = r(t) + gamma.i(t).dt here gamma is removed from the infacteds per days. loss of susceptible is gain for infecteds. loss rate of infacted people is just a constant probability of recovery.
