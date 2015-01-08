C2D Pre-Release
===
###Model of Design-Team Formation and Collaboration on a NK Design Landscape 

<br>
<br>


![alt text] (http://static.tumblr.com/ywmlmzw/6h5m2qllb/vt-logo-transparent-1200x258.png)

# Virginia Tech System Performance Lab  


## WHAT IS IT?

This model demonstrates the process of collaborative and value-centric design for engineered sociotechnical systems across a technology possibility space, a design possibility space.  The model generates this design possibility space, conceptually similar to an economic production possibility space, via a fitness landscape.  The resulting design landscape provides a generalizable representation of various potential designs (i.e. points in the design possibility space) and their corresponding fitness (e.g. value).  This model builds on models by Uri Wilensky (2007a, 2007b) and David McAvity (2006). The resulting model enables the study of and demonstrates:

- <b> Lateral Alignment in Collaborative Networks </b>
-- Analogy of mutation allows us to explore when and how lateral alignment within a design team (i.e. incorporating disciplines and backgrounds outside of current team makeup) may lead to an improved design (e.g. value) and to what extent.
- <b> Collaborative Networks on a Landscape with an Augmented Hill Climbing Approach </b>
- <b> Value-centric Design as a Fitness Landscape </b>
- <b> Design Teams and Collaborative Design Teams </b>
   
## HOW IT WORKS

Theoretically the fitness landscape shown corresponds to a NK-fitness landscape model where ruggedness of the space is determined by the smoothness variable (a composite of the NK values in the NK-fitness landscape).  The surface in the model has both smoothness (i.e. degree patch neighbors have equivalent range values) and range characteristics (i.e. height or fitness); in addition, the number of components, N, from the NK theory relates to the dimensionality of the world.  The model places agents (e.g. designers) into this resulting design landscape where they create collaborative networks that navigate the space using the hill climbing procedures and other management strategies.   The landscape also provides a representation of a phenotype space, from biological sciences, where the attributes of fitness are binomial (e.g. quality and cost as an example in design).

These design agents also interact with their environment and are subject to their own fitness.  In this application, how long an engineer would spend exploring options depends on its fitness (i.e. less time is spent on designs with less fitness).  This has a biological comparison of natural selection (i.e. the fitness of real organisms is related to the probability of surviving until reproductive age and creating offspring). This natural selection pressure relates to the fitness of the agents location in the design space (i.e. a design concept), aside from this influence the model assumes each collaboration agent has the same probability to move and influence the design forward.  

Additionally, the model allows the landscape to change with time; this allows the model to demonstrate the importance of collaborations to continually explore their design space, especially in high flux work environments.  The changes in this landscape represent many activities for the designers and their collaborators; these changes may mean modifying or changing design configurations as requirements change (e.g. Engineering Change Proposals).  And, at a further abstracted level of the analogy, this changing landscape also demonstrates the need to develop organizational entities to pursue new technical systems as previous designs face obsolescence. 

To accomplish the creation of this model, we combine aspects from several well-studied models.  These included building on modeled concepts from collaborative network formation and extending these essential team dynamics into the domain of biological fitness landscapes.  In particular, the adapted model leverages a team assembly model presented by Guimera, Uzzi, Spiro, & Amaral (2005) and remixes elements of the Uri Wilensky model (2007).  

In this model at each tick a new team is assembled and the members of the team are either inexperienced "newcomers" or are established "incumbents" who were previous participants (i.e. on the team more than once).  The likelihood that a new team member is choosen is given by the slider bar in the user interace. 

Similiarly, the team may appoint an incumbent with a given probability.  If possible the team will try to select an incumbent  from the current team; however, if there are no currently available team members that are incumbents the team will appoint previous collaborators from the network to join the team.  The probability of this occurence is dictated by a slider bar in the user interface.  

This application of this team concept extends the collaborative model onto a design fitness landscape.  At each tick that a new team member introduces a "newcomer" it does so with a distance equal to a random value up to the mutagenic distance input by the user. This concept of mutagenic distance represents conceptual alignment, the further the mutagenic distance the more relevant diversity and skillsets that a group is willing to integrate into its collaboration.

In the model, newcomers are colored blue and incumbents are colored yellow.  The blue links similiarly represent the interactions between two newcomers, green links represent newcomer-incumbent interactions, yellow links represent incumbent-incument collaborations, and red links indicate repeate collaborations between designers. These links are established at the most recent collaboration (i.e. the links are determined when the agent is actively engaging as part of the core team).  As alluded in the past, the fitness of the space around a current collaborative design-team space dictates the likelihood that a team member will be able to introduce a "newcomer" and the mutation rate dictates the likely conceptual diversity that a "newcomer" will bring to the team.  

Other strategies aside from these mechanics, such as the use of a traditional hill climbing procedure are enabled in the model via user selection.  This model adopts as its defaults techniques from the research that have shown to be effective in driving the design process.  In particular this means using a modified form of this hill climbing approach (i.e. the coalesce? input), an approach that searches out the landscape for peaks but while also allowing for natural selection processes to drive the process when no known peak to the collaboration meets the requirements of the design. Furthermore, this set of default strategies also entails making use of a dynamic mutation rate, a rate that dictates, in this model, the willingness of the group to incorporate diverse team members.  This rate changes with time to adapt to the situation the group faces. Other userful models strategies include the possibility of dynamically ramping up the selectivity required for continuing on a partiuclar design (i.e. reproduction), essentially this conceptually may represent a design manager's pressure to bring about consensus.  This tool helps to address issues where multiple competing peaks makes the final selection of a design too timely for the design process (in biological terms this helps to alleviate allopatric speciation). 

## HOW TO USE IT


Like most NETLOGO models, this model requires the user to setup and run the model.  These basics interfaces of the model include <i> setup </i> and <i> go </i>.  Other user defined inputs allow the user to change aspects of the team composition, mutation (<i> aspects of later alignment </i>), adaptability of the agents (<i> designers </i>), and aspects of the fitness landscape (<i> design possibility space </i>).

### <i><b> Basics </i></b>
- <b> Restore Defaults: </b> Press button to restore default settings for simulation (hotkey: D)
- <b> Setup: </b> Press button to clear simulation and before beginning (hotkey: S)
- <b> Go: </b> Press button to run or pause simulation (hotkey: G)
-- <b> Go Once: </b> Press button to run the simulation for one tick (hotkey: 1)
- <b> Spring Layout Once: </b> Press button to run the spring layout algorithm once per click to visualize network, this should be down after the simulation has completed so it doesn't influence the results (hotkey: R)
-- <b> Visualize with black world output: </b> Press this advanced control button or use its hotkey to better visualize the network by turning the design space black (hotkey: V). This is irreversible per run and, although it does not influence the running of the model, it should be run at the conclusion of the simulation with the Redo Layout routine (hotkey: R).
-- <b> Spring Layout Continuously: </b> Press button or use hotkey to continually run the layout algorithm to optimize the display of team. This should be done after completing the simulation only and turned off after the visualization optimization is complete (hotkey: O)
-- <i> Note: </i> Ensure that the Redo Layout Continuously option is not running before running the simulation as this is a button, user-interface option it cannot be reset by restoring defaults




### <i> <b>  User Inputs </i> </b>

#### Basic Inputs

- <b> Team-Size: </b> Number of team-members for the collaborative network (default 4)
- <b> prob_of_newcomer, <i>1-p</i>: </b> Probability of choosing a newcomer to become a team member (default 24%)
- <b> propensity_to_repeat_collaboration: </b> Probability of an incumbent to repeat a previous collaborator (default 82%)
-- <i> If there are no available incumbents then, even with no propensity, repeat collaborations may occur
- <b> Mutation: </b> Maximum distance a collaborator hatches from an agent in the team (default 10)
- <b> Max-downtime?: </b> Allowable time with no collaborating (default 40)
- <b> Stopping-fitness: </b> Acceptable design fitness (default 92)

#### Advanced inputs

- <b> Smoothness:  </b> This slider bar tunes the ruggedness of the landscape (default 70)
- <b> Range: </b> This slider bar dictates the relative heights of peaks (default 100)
- <b> Changing-landscape?: </b> This switch enables the landscape to change (default off)
- <b> Landscape-change-rate: </b> This slider allows you to vary the dynamism of the landscape change (default 200)
- <b> Max-downtime?: </b> Keep the dynamic of maximum downtime in a team (default on)
- <b> age?: </b> This introduces the natural selection component, those who age out cannot produce and (default on)
- <b> hill_climbing?: </b> This introduces the use of a traditional hill climbing approach to searching the design landscape (default off)
- <b> coalesce?: </b> This introduces a modified hill climbing approach by allowing the team to search out the space looking for a peak, if the peak does not meet the fitness requirement the process of natural selection drives the continued search.  This approach allows the team to use the hill climbing concept to locate peaks and natural selection when the only nearby peaks aren't acceptable solutions.  This will allow the team to evolve together toward singular peaks (default on)

#### Alternate model parameters and inputs

- <b> Cobb-Douglas?: </b> This option allows the user to switch to a convex production possibility space that allows for study under the axiomatic assumptions of production theory (default off)
--  If this is enabled additional options allow the user to vary the coefficients, total production factors, and elasticities of production.  


#### Major Strategies

- <b> require_same_stop_point: </b> This option requires that both the core team and collaborative body as a whole come to an approximate agreement on the approach before selection (default on)
- <b> dynamic_mutation: </b> This option varies the diversity of a candidate the team is willing to recruit from depending on the current situation and progress of the design. This will continue to ramp up mutation until a stopping condition is reached or the maximum mutation (i.e. the diagnol distance of the world) is reached (default on)
- <b> pause_restart_mutation?: </b> This option will, upon reaching a maximum threashold of mutation, restart the mutation - giving the team an opportunity to reasses its skill mix and team diversity (default on)
- <b> stop_mutation_if_fit?: </b> This option will reset mutation to zero if the team has realized a fit solution (default on)
- <b> stop_prolonged_decisions: </b> This option will ramp up the unfitness penalty when more than one acceptable peaks appears (if no peaks, when two acceptable better points) are found (default off)
-- <i> The unfitness penalty below is the default rate for this penalty (default 1) </i>
-- <i> Depending on experimental setup, this maybe defaulted to on </i>


### <i> <b> Visualization Controls </i> </b>
- <b> Spring_Layout?: </b> This button enables the experimenter to visualize the network using the Fruchterman-Reingold layout algorithm at each increment of time or tick.  This procedure allows the nodes to move around to make the structure of the collaboration network easier to see (default off)* 
--<i>Switching off LAYOUT? significantly increases the speed of the model and is recommended for analytical purposes</i>
--<i>Running the model with the LAYOUT? ON also represents the need for designers to have their own autonomy to explore to some degree on their own - this is modelled using the spring constant options, but represents an area for consideration </i>
--- <b> Spring Layout Once: </b> Enables the ability to run the layout algorithm once per click at any time, including after the simulation has been completed, and allows the experimenter to visualize the current state of the network (hotkey R)
--- <b> Spring Layout Continuously: </b> Press button or use hotkey to continually run the layout algorithm to optimize the display of team. This should be done after completing the simulation only and turned off after the visualization optimization is complete (hotkey: O)
--- <b> Visualize with black world output: </b> Press this advanced control button or use its hotkey to better visualize the network by turning the design space black (hotkey: V). This is irreversible per run and, although it does not influence the running of the model, it should be run at the conclusion of the simulation with the Spring Layout Once routine (hotkey R) or Spring Layout Continously (hotkey O).


### <i> <b> Advanced Controls and Strategy </i> </b>

These controls allow the user to modify core elements of the model (e.g. aging process, down-time limitations, hill climbing method for searching out fitness) and allows the user to try out potentially useful strategies.  These strategies are experimental attempts to simulate concepts, such as punctuated equilibrium.  In this particular strategy, the team increasingly seeks collaboration farther outside of its current thinking locus (i.e. it increases its mutation rate) while also assessing its current progress.  It increases it up to a maximum and if it still hasn't achieved success it focuses on its current location, and then increasing mutation in a loop untill it has achieved success.  Other various strategies conceptually relate to group consensus and agreement.


## THINGS TO NOTICE

#### Collaboration Networks & Team Dynamics

The model captures the basic features of collaboration networks that can influence or stifle innovation in creative enterprises, the relative compositions of a collaborative team. The type of team members (i.e. experience/familiarity) most likely to join the collaborative effort are varied in the model through the values <i>p</i> and <i>q</i>. 

The first of feature captured by the model is characterizing the distribution of the type of the connection between collaborators.  This distribution can be seen in the <b>Link Type plot</b>, and is one of the clearest indicators into the probability of success for a team (Guimera et al. 2005). An overabundance of newcomers (seen in the newcomer-newcomer blue colored links and agents) might indicate that a field is not taking advantage of experienced members or that no experienced members are available. On the other hand, a multitude of repeat collaborations (orange colored agents) and incumbents (seen in the incumbent-incumbent yellow colored links and agents) may indicate a lack of diversity in ideas or experiences.

The second essential feature captured in the model is characterization of the connectivity of the collaboration network. For example, Wilensky (2007a) points out that some consider many academic fields as comprised of an “invisible college” of loosely knit academic communities. Conversely, other communities, such as patent networks, tend to consist of isolated clusters or chains of inventors. This measure is taken as the percentage of agents in the large connected chain of collaborators and is seen in the <b>Core Agents plot</b>.

The model allows the experimenter to visualize the emergent networks of interactions and their topologies as these teams navigate the fitness landscape. New collaborations or synergies among teams naturally tend to the center of the display, in the traditional model.  However, this model uses the hill climbing algorithm and the fitness landscape to move the collaborative network across the design possibility space. Teams or clusters of teams with few connections to new collaborations naturally “float” away from the current collaboration. Newcomers always hatch near a current agent if mutation is turned off; however, if mutation is enabled the new-comer will come from a different location on the fitness landscape and will have his own fitness (e.g. design idea) to contribute and can help move the group. Incumbents, which are chosen at random, may be located in any part of the landscape. Thus, collaborations amongst newcomers and or distant team components tend toward the network in the absence of mutation and disconnected clusters are repelled.

Finally, note that the structure of collaboration networks in the model can change dramatically over time. Initially, only new teams are generated as the collaborative effort has not existed long enough for members to retire or lose interest / ability to contribute (two factors influence the death of an agent, <i>age</i> and <i>downtime</i>). However, after a period of time <b>max-downtime</b>, inactive agents begin to retire and <b>age</b>, as a result the number of agents becomes relatively stable.  The emergent effects of <i>p</i> and <i>q</i> become more apparent in this equilibrium stage. The end of the growth stage is often marked by a drop in the connectivity of the network Wilensky (2007a); this drop in connectivity is also compounded by the fact that agents (i.e. designers) that are <i>less fit</i> (i.e. pursuing suboptimal design) have less opportunity to produce in the model because they die out sooner.


#### Fitness Landscapes

A fitness landscape is often used to visualize the relationships in the biological sciences to represent relationships between genotypes and the likelihood of reproductive success in a species (i.e. <i> fitness </i>).  However, more recently the use of these landscapes have been applied in economic and performance measurement literature (Triantis and Keller, 2013).  In particular the NK landscape developed by Stuart Kauffman and Eric Weinberger (1989) provides for a tunable rugged fitness landscapes that has proven valuable in evolutionary biology, immunology, optimization, and organizational theory.  

In general in the NK model, <i>N</i> is the number of characteristics or parts of an organization (e.g. cost, quality).  Each of these <i>N</i> characteristics exist in <i>A</i> number of states.  This <i>A</i> to the power of <i>N</i> can be represented in a binary string with fitness values randomly assigned.  Finally, <i>K</i> represents the interdependence from zero to <i>N - 1</i>, with <i>N - 1</i> being maximally interdependent (i.e. each characteristic is affected by all the other characteristics).  In this model the parameters for roughness and range roughly approximate these tunable characterstics.

In our landscape, if each agent were unconstrained by a collaborative network the agents would gradually drift-up up the fitness landscape to local fitness peaks, although frequently groups of turtles may survive for a time away from the peaks. In this case, these groups would represent less than optimally fit subgroups who survive by random chance. In our case and in this simulation, the networks may also fluctuate and, in fact, become stuck in local minimum as well.

The <b>Average Fitness of Team</b> plot shows the average fitness of the team (i.e. fitness of emerging design concept), but with some fluctuations due to team members. 

The landscape can also lead to <i>genetic drift</i> events when the team is forced into two groups where one will die out, even if both groups have similar fitness (sometimes a fitter subgroup may die out as a result). 

#### Hill Climbing 

This algorithm makes turtles climb hills (i.e. follow the gradient of the environment).  It utilizes the <i><b>UPHILL</b></i> command, which makes the turtle examine its eight neighboring patches and move to the center of the patch with the highest value (in the event of a tie, NetLogo breaks the tie randomly). 

-- When the mutation is set to zero and there is no dynamic mutation strategy enabled, you can notice the frequency that agents get stuck in attractors that are local minimums and sticking points that are less than the desired design performance/value (i.e. stopping-fitness).

## DISPLAY AND MONITOR NOTES

### Team Characteristics
- <b> Incumbent Pool: </b>  Displays the current number of possible incumbents, this number includes newcomers not currently on the team (i.e. eligible to become incumbents) and those that have already become incumbents (i.e. been on the team multiple times) 
- <b> Team Newcomers: </b> Newcomers currently on the team (this is the first time the agent has participated in the team)
- <b> Team Incumbents: </b> The number of repeat participants currently on the team
- <b> # Collaboration Incumbents:</b> This value is the number of collaborators currently in the network who have participated in the team multiple times
- <b> # Collaboration Newcomers: </b> This value is the number of newcomers currently in the network, these agents have only participated in the team once when they first joined the collaborative effort
- <b> # Repeat Collaborators: </b> This is the current number of agents in the collaboration that are engaged in a repeat collaboration (i.e. they have collaborated with the agent more than once)

### Network Characteristics 
- <b> Avg. Clustering Coefficient: </b> This reports how clustered the network is on average
- <b> Connectedness: </b> This reports how many links there are relative the maximum theoretical number of links to be fully connected (cf. Metcalf's Law)
- <b> Avg. Path Length: </b> This reports the average length of the links


## THINGS TO TRY

Explore the relationships between the variables of group dynamics and the fitness landscape to gain insights into the interactions between teams and their environments.

## EXTENDING THE MODEL

Future research hopes to more explicitly treat aspects of path-dependence (i.e. how does the initial placement of the agents in the design space influence outcomes).  


## RELATED MODELS

<a href="http://ccl.northwestern.edu/netlogo/models/community/Fitness_Landsacape"> McAvity, D."Fitness Landscape" (2006) </a>

<a href="http://ccl.northwestern.edu/netlogo/models/TeamAssembly"> Wilensky, U. "Collaborative Team Assembly" (2007a) </a>

<a href="http://modelingcommons.org/browse/one_model/2256#model_tabs_browse_discuss">Wilensky, U. "Hill Climbing Example" (2007b) </a>


## CREDITS AND REFERENCES

Bakshy, E. and Wilensky, U. (2007). NetLogo Team Assembly model. http://ccl.northwestern.edu/netlogo/models/TeamAssembly. Center for Connected Learning and Computer-Based Modeling, Northwestern University, Evanston, IL.

<a href="http://amaral.northwestern.edu/Publications/Papers/Guimera-2005-Science-308-697.pdf"> R Guimera, B Uzzi, J Spiro, L Amaral; Team Assembly Mechanisms Determine Collaboration Network Structure and Team Performance. Science 2005, V308, N5722, p697-702  </a>

Teahan, W. J. (2009). Artificial Intelligence. Ventus Publishing Aps

Wilensky, U. (1999). NetLogo. http://ccl.northwestern.edu/netlogo/. Center for Connected Learning and Computer-Based Modeling, Northwestern University, Evanston, IL.

## LICENSE INFORMATION

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/deed.en_US"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png" /></a><br />

To collaborate for on this model and its adaptations or source derivations:

http://ccl.northwestern.edu/netlogo/
http://www.sdl.ise.vt.edu/ 
http://www.ise.vt.edu/ResearchFacilities/Labs/LabPages/SP_lab.html
   
