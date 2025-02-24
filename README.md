Download link :https://programming.engineering/product/homework-2-the-return/

# Homework-2-The--return
Homework #2 The -return
Problem

1.1 Description

Given an MDP and a particular time step t of a task (continuing or episodic), the -return, Gt , 0 1, is a weighted combination of the n-step returns Gt:t+n, n 1:

1

Gt = P (1 ) n 1Gt:t+n:

n=1

Whereas the n-step return Gt:t+n can be viewed as the target of an n-step TD update rule, the -return can be viewed as the target of the update rule for the TD( ) prediction algorithm, which you will become familiar with in project 1. Note that the n-step return Gt:t+n is functionally equivalent to the k-step estimator Ek from the lectures if we set k = n and estimate the value of the state the agent is in at time t.

Consider the Markov reward process described by the following state diagram and assume the agent is in state 0 at time t (also assume the discount rate is = 1).


A Markov reward process can be thought of as an MDP with only one action possible from each state (denoted as action 0 in the gure above).

1.2 Procedure

You will be given p, the probability of transitioning from state 0 to state 1, V, the estimate of the value function at time t, represented as a vector [V (0); V (1); V (2); V (3); V (4); V (5); V (6)], and rewards, a vector of the rewards [r0; r1; r2; r3; r4; r5; r6] corresponding to the MDP.

Your goal for this homework is to nd a value of , strictly less than 1, such that the expected value of the -return equals the expected Monte-Carlo return at time t.

Provide answers for the speci c problems you are given on Canvas. Your answer must be correct to 3 decimal places, truncated (e.g. 3.14159265 becomes 3.141).

{ The -return

2

Examples

The following examples can be used to verify that your agent is implemented correctly.

Input : p = 0:81; V = [0:0; 4:0; 25:7; 0:0; 20:1; 12:2; 0:0]; rewards = [7:9;-5:1; 2:5;-7:2; 9:0; 0:0; 1:6] Output : 0:622

Input : p = 0:22; V = [12:3;-5:2; 0:0; 25:4; 10:6; 9:2; 0:0]; rewards = [-2:4; 0:8; 4:0; 2:5; 8:6;-6:4; 6:1] Output : 0:519

Input : p = 0:64; V = [-6:5; 4:9; 7:8;-2:3; 25:5;-10:2; 0:0]; rewards = [-2:4; 9:6;-7:8; 0:1; 3:4;-2:1; 7:9] Output : 0:207

Resources

The concepts explored in this homework are covered by:

3.1 Lectures

Lesson 3: TD and Friends

3.2 Readings

Chapter 7 (7.1 n-step TD Prediction) and Chapter 12 (12.1 The -return) of R. S. Sutton and Barto 2020 R. Sutton 1988

Submission Details

The due date is indicated on the Canvas page for this assignment.

Make sure you have set your timezone in Canvas to ensure the deadline is accurate.

Submit your answers on Canvas, as outlined in section 1.2. You will have a total of 10 submission attempts – only the highest score is kept.

References

[SB20] Richard S Sutton and Andrew G Barto. Reinforcement learning: An introduction. 2nd Ed. MIT press,

2020. url: http://incompleteideas.net/book/the-book-2nd.html.

[Sut88] Richard Sutton. \Learning to Predict by the Method of Temporal Di erences”. In: Machine Learning 3 (Aug. 1988), pp. 9{44.
