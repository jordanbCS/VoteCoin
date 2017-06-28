# VoteCoin
##Public repository of VoteCoin.com

Currently a mix of Matlab, latex and markdown


##[candidateSizedField] = VoteField##({a 1d set of candidates $c$ indexed by $j$})

Votes for a candidate are weighted by the continually accruing and spending of identity trust, where: $v_i(t) = v_i + \tau n_{aff}/n_{eff}(-v_i + -eff + aff)$ This is the amount of influence that a voter $i$ can exert when voting for their chosen candidate. A sum will  be taken across all of the weighted voters to figure out the activation of their chosen candidate. A VoteField is initialized when:

1. Each voter $i$ generates a private key.  

2. Voters form groups of size $c$ with their friends irl, and share secrets 
$s_{i,j}$ with each of them.  

3. Shared secrets define individual specific identity kernels.



###efferentVoteField###({a 2d set of voter x candidate ranks})

An efferentVoteField is characterized by the way its members pulse to one another in order to maintain positional indicators. This is the "vote", for the direction of payout of the votemine comes every $\tau$ days. A voter will pulse the direction of the candidate, with obfuscation of specific voter intentions generated by including hashes of rank preferences along with the modified believed outcome of the election by the voter. The VoteField maintains the integrity of the results by sharing a secret with each voter that includes their hidden votes + public hashes, and propagating its existing activation in a direction slightly altered toward that voter's preferred candidate which will subsequently influence which voters are queried next. 



efferentSpaceField({{a set of nodes with their subgraphs of direction/magnitude subgraphs}

1. Every candidate node gets an activation energy at time $t$.

2. The preferred candidate rank opinions $c$ of a voter $i$ can be thought of as pointing to a location in a candidate space: $c_j = v_{i,j}\sigma(i)$.

3. A dynamically adjusted timestep (e.g. 4 years), sees a similarity kernel applied the weighted sum of inputs for each candidate given the squashed ranks received for each voter. 

4. We can dispense with setting timesteps to constants by updating only when some weighted inputs are high enough to cross a threshold: something like a leaky accumulator. 

5. Lower ranking candidates are shifted toward lower positions on the field by the matching updated preferences of the candidate for their voters as part of creating the metric for the field. 


\section{Thoughts}

Still many vagaries.
