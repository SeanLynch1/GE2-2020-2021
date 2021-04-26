# Game Engines 2 2020-2021

[![Video](http://img.youtube.com/vi/KNymjRyr27A/0.jpg)](http://www.youtube.com/watch?KNymjRyr27A)

## Teams links for classes:
- [Tuesday 9am lab](https://teams.microsoft.com/l/meetup-join/19%3ameeting_MzhhZmVhY2MtOWI5Ni00ZjExLTliYmMtZWJiZjhjYTVkYmY5%40thread.v2/0?context=%7b%22Tid%22%3a%22766317cb-e948-4e5f-8cec-dabc8e2fd5da%22%2c%22Oid%22%3a%2261aab78b-a857-4647-9668-83d4cca5de03%22%7d)
- [Thursday 11am Class](https://teams.microsoft.com/l/meetup-join/19%3ameeting_YjdhMGNhZDYtOTU4MC00YjViLTk5MjQtOWFlZDk5MDM4ZTYw%40thread.v2/0?context=%7b%22Tid%22%3a%22766317cb-e948-4e5f-8cec-dabc8e2fd5da%22%2c%22Oid%22%3a%2261aab78b-a857-4647-9668-83d4cca5de03%22%7d)
- [Friday 10am Class](https://teams.microsoft.com/l/meetup-join/19%3ameeting_MmU0OTg2YWMtOWQ0YS00YzA2LTk0NmQtMTczNjM0MTczNzY5%40thread.v2/0?context=%7b%22Tid%22%3a%22766317cb-e948-4e5f-8cec-dabc8e2fd5da%22%2c%22Oid%22%3a%2261aab78b-a857-4647-9668-83d4cca5de03%22%7d)

## Resources
- [Class Facebook page](https://www.facebook.com/groups/407619519952058/)
- [Assignment](ca.md)
- [A build of Infinite Forms](https://drive.google.com/file/d/1w24BcMAi6P1XmPc9D9ss6Lkro4KBvsMS/view?usp=sharing)
- [All about Infinite Forms](http://bryanduggan.org/forms)
- [A spotify playlist of music to listen to while coding](https://open.spotify.com/user/1155805407/playlist/5NYFsIFTgNOI93hONLbqNI)

## Contact me
* Email: bryan.duggan@tudublin.ie
* Twitter: [@skooter500](http://twitter.com/skooter500)
* [My website & other ways to contact me](http://bryanduggan.org)

## Previous years courses
- [2019-2020](https://github.com/skooter500/GE2-2019-2020)
- [2018-2019](https://github.com/skooter500/GE2-2018-2019)

## Previous years lab tests
- https://github.com/skooter500/GE2-Lab-Test-2019
- https://github.com/skooter500/GE2-Lab-Test-2019-Solution
- https://github.com/skooter500/GE2-LabTest2-2017
- https://github.com/skooter500/GAILabTest12017
	
## Assessment Schedule	
- Week 6 - CA proposal & Git repo
- Week 12 - Tuesday 27th April 9am Lab Test - 20%
- Week 13 - Friday 7th May CA Submission - 50%
- 17 May 2021 2pm-5pm - End of year online test

## Week 12 - Path Finding and A*
- A* in C#
- Navmesh

## Week 11 - Flocking in ECS
- [Video of Thursdays class](https://www.youtube.com/watch?v=0ByqDsfdblY)


Friday

Exercise! 

- Check out Avoidance scene
- How are the feelers calculated?
- What direction do they point?
- How many are there? Whys this number?
- How does the behaviour handle holes in the colliders?
- Does the speed of the boid matter?
- What direction is the force generated?
- WHat alternatives are there to this?
- How does the behaviour avoid certain obstacles while ignoring others?
- How often are the feelers calculated and why?
- How does the behaviour take priority over other behaviours?
- How would you improve the behaviour?
- How does it improve on Craig Reynolds avoidance behaviours?

- [![YouTube](http://img.youtube.com/vi/qmtxqCU1X5Q/0.jpg)](https://www.youtube.com/watch?v=qmtxqCU1X5Q)

Thursday

Have a look at the PureECSScene in [this repo](http://github.com/skooter500/ECS2020) and answer the following questions:

1. What are Entities, Components, Systems and Jobs?
5. What is the purpose of the class BoidBootstrap?
2. In the previous examples, we explored two approaches to creating Entities. Describe them. Which approach was used in the PureECSScene Scene?
3. How many systems are there running in PureECSScene? What are they and what do they do?
4. In the previous examples we looked at two different types of jobs. What were they and what were they for? 
4. BoidSystem schedules IJobEntityBatch jobs. What are these and how does this approach differ from using Entities.ForEach? 
4. How do these jobs selects Entities to iterate over? How are the Components on these Entities accessed? 
6. What is a Native Container? Give some examples. What Native Containers does the BoidSystem create and what is their purpose?
7. What Jobs does the BoidSystem schedule and in what order. Is this order significant?
8. PartitionSpaceJob uses an algorithm called Cell Space Partitioning. How can this algorithm reduce the computational complexity the Flocking?
9. What is the limitation of this algorithm?
9. How are Boids assigned cells?
10. PartitionSpaceJob uses a NativeMultiHashMap. What is the purpose of this data structure? What is the computational complexity of retrieving a value from a key in this data structure?
10. How do Boids access the positions and rtotations of other Boids?
11. In CountNeighboursJob, how does the algorithm determine how many cells are surrounding a boid that it needs to check for neighbours?
12. What is the design pattern for retrieving all the values that match a given key in a NativeMultiHashMapIterator?
13. Where does the algorithm store the neighbours for each Boid?
14. What happens if a Boid has too many neighbours?
15. In SeperationJob, what can cause the force to be NAN? How does the code check for this?
16. How does Cohesion work?
17. In AlignmentJob how are the forward vectors for each boid calculated?
17. How is the desired forward vector calculated?
18. How is the force generated?
18. What algorithm does BoidJob use to combine the forces from the various behaviours together?
19. How is the Boids rotation evaluated?
20. In SpineSystem, what is the purpose of the WithNativeDisableParallelForRestriction annotation on the Entities.ForEach lambda?
21. What jobs does SpineSystem schedule and what do they do?
21. What parameters control the damping on the spine and what effect will changing these parameters have on the spines?
21. What Native Containers does this job create?
22. In HeadAndtailsSystem, what controls the speed of the procedural animation?
22. How does the Head Animation work? Draw a diagram. What Unity API call is this system similar to?

[![YouTube](http://img.youtube.com/vi/8J7rliGiKw0/0.jpg)](https://www.youtube.com/watch?v=8J7rliGiKw0)

## Week 10 - ECS Boids

- [Video of Thursday's class](https://web.microsoftstream.com/video/367c5760-bd8e-473e-b41b-7e42f5c5ff47?list=studio)
- [Video of Friday's class](https://web.microsoftstream.com/video/725de1c7-8801-4658-bc23-715c4b9b9d67?list=studio)

## Week 9 - Entity Component System - Cellular Automata & Psytrance Spirals

[![YouTube](http://img.youtube.com/vi/KNymjRyr27A/0.jpg)](https://www.youtube.com/watch?v=KNymjRyr27A)

## Lecture
- [Video of Thursday's Class](https://web.microsoftstream.com/video/d962ebfb-8bd2-4ff5-bec9-c136c57c5e7b)
- [Video of Friday's Class](https://web.microsoftstream.com/video/c889ecca-1c83-4ad0-9230-d76d0a438cd5)

## Lab
- [Cellular Automata in ECS Lecture](https://web.microsoftstream.com/video/4e9fb74b-e903-4180-ba2e-2d21bf94404f?list=studio)

## Week 8 - Entity Component System - Voxel terrain * Cellular Automata in 2D & 3D

## Lecture
- [Thursday's class](https://web.microsoftstream.com/video/745bc27c-5628-440a-99b1-6cd677bdf9eb?list=studio)
- No class on Friday due to power cut

## Lab
Fork and clone the [ECS2020 repo](https://github.com/ECS2020). It has the code we worked on in Friday's class, with some improvements I made (we will talk about these on Thursday). The scene we worked on now looks like this:

![Image](https://bryanduggandotorg.files.wordpress.com/2021/03/noise00001.png?w=895&h=&zoom=2)

Currently, there are 10K entities being created and destroyed. This is a pretty inefficient way to generate a terrain from perlin noise! Much better would be to create a single Entity with a mesh and update the mesh vertices in a job. I started work on implementing this approach in the branch mesh_deformation. I got a script online that generates a plane mesh. It's in the scene MeshDeformation. I added some Perlin noise to the mesh just to test that it was being generated correctly. You can try and finish the job by creating a single entity that renders the mesh and writing a job and a system to update the vertices. This will involve some looking at code and googling stuff! Here is what I suggest you do:

- Fork and clone the repo
- Checkout the mesh_deformation branch
- Create a new branch for your work called week8lab
- Look at the code in NoiseCube, you will see an example of how to create entities and how to write a system
- Create a system in the file meshController.cs and call it MeshDeformer
- Create a component with no fields, an archetype and an entity
- Create a NativeArray of type Vector3 to hold the mesh vertices
- Write a a job that iterates over the NativeArray and updates the vertices
- Every frame, copy the NativeArray of vertices back to the mesh

Someone has done something similar with jobs, but not entities in [this repo](https://github.com/adcimon/unity-job-system-mesh-deformer), so might be worth having a look.


## Week 7 - Entity Component System
## Lecture
- [ECS Slides](https://drive.google.com/file/d/1nGoqxueagIqOwTWA7TZ7NpVYfKwhrIMV/view?usp=sharing)
- [Video of Thursday's class](https://web.microsoftstream.com/video/6ab9cb85-3684-4bf9-a90b-2a7b2257a8f6?list=studio)
- [Video of Friday's class](https://web.microsoftstream.com/video/4128090f-b5db-482e-8794-9a702fb57aba?list=studio)
- [My ECS repo](https://github.com/skooter500/ECS2020)
- [Official ECS Samples](https://github.com/Unity-Technologies/EntityComponentSystemSamples)


## Lab
### Learning Outcomes
- Learn how to use the state machine design pattern
- Learn how to draw a FSM diagram
- Get the ECS examples working

## Part 1

In this video are the two autonomous agents we programmed in Friday's class with some enhancements and additional states you can make today:

[![YouTube](http://img.youtube.com/vi/R6yzjthBH4U/0.jpg)](https://www.youtube.com/watch?v=R6yzjthBH4U)

The blue agent goes between Patrol and Defend states. In Patrol state, the agent will follow it's path. In defend state, it will fire at the green agent until either it runs out of ammunition or the green agent goes out of range. The green agent will go between it's Attack state, where it will fire at the blue agent or Flee state where it will flee from the attacking blue agent. 

If an agent runs out of ammunition it will locate and pickup the nearest ammunition. These are tagged with "Ammo".

If an agent gets below 2 health, it will locate and pickup the nearest health. These are tagged with "Health".

The spawning system keeps 5 health and 5 ammo in the scene at all times.

If an agent gets to 0 health, it goes to the Dead state. In Dead state, the state machine gets turned off and all the steering behaviours get disabled.

Update your forks of the repo from my master branch and make a branch for your work today. All the above is in a scene called StateMachines. The states are in the file States.cs.

To complete the lab:

- Make an Alive state that checks health and ammo levels and transitions to GetHealth, GetAmmo or Dead as appropriate
- Make this the Global state for each agent
- Make GetHealth, GetAmmo states with Enter, Think and Exit methods. When transitioning out of GetHealth and GetAmmo, use RevertToPrevious in order  to implement these as state blips.
- Modify Attack and Defend states so that they remove ammo when shooting
- Draw state transition diagrams for both agents.

Other things to try:

- Modify the targeting
- Try Evade instead of flee
- Make the agents opportunistic. I.e. An agent will not only seek health or ammo when it gets low, instead if an ammo or health happens to come in range, the agent will try to get it
- Increase the complexity of the scenario by adding additional states

## Part 2 - If you have time!

In case you are curious, here is the video of Psytrance Music Visualiser:

[![YouTube](http://img.youtube.com/vi/KNymjRyr27A/0.jpg)](https://www.youtube.com/watch?v=KNymjRyr27A)

And here is a [blog post](https://bryanduggan.org/2021/03/04/psytrance-spiral-generator/) with some screenshots. It is one of the Entity Component System samples I am putting together for the course. It generates a great variety of beautiful spirals and can be beat tracked to the audio.

You can [check out the repo](http://github.com/skooter500/ECS2020) in advance of this weeks class.

## Week 6 - Finite State Machines

### Lab
- [Submit the github repo for your assignment](https://docs.google.com/forms/d/e/1FAIpQLSf8XGjtZjvkVs7NTt9gOq3H2ls7VryCiwH2uVhHWTWxxycv1g/viewform)
- Make a behaviour called Constrain that keeps a boid inside a sphere of interest. If the boid goes outside the sphere, generate a force to push the boid back towards the centre of the sphere.
- Make some creatures with NoiseWander, Harmonic, Constrain and the SpineAnimator 

### Lecture
- [Thursdays' class](https://web.microsoftstream.com/video/f89bdaae-26c9-4e39-9f36-0ec5f108faa5?list=studio)
- [Friday's class](https://web.microsoftstream.com/video/4426c2dc-eb00-47bb-b869-e6a506adf6a9?list=studio)

## Week 5 - Harmonic & NoiseWander behaviours
### Lecture
- [Video of the class on Thursday](https://web.microsoftstream.com/video/d27e6703-6350-4fa4-8345-532837de2cdb)
- [Video of the class on Friday](https://web.microsoftstream.com/video/bb01cfa3-cdcb-4036-b30c-4db2c891a0e0)
- [A playlist of my creatures]()

### Lab
A few ideas for todays lab!
1. Clone [this repo](https://github.com/skooter500/ECS2020) and check out my ECS experiments. If you feel like a challenge, fix the bug in the Life scene. In this scene I am attempting to program a 3D cellular automata (like the Game of Life) in 3D
2. [Try this lab test](https://github.com/skooter500/GE2-Lab-Test-2019)
3. Work on your assignment. The first deliverable is due next week

## Week 4

### Lecture
- [WTPRS & Wander](https://web.microsoftstream.com/video/b6945686-bc22-4d0b-b071-abe4c63130e1?list=studio)
- [Unity Input System (presented by Tadhg O Rourke)](https://web.microsoftstream.com/video/b2abfc9b-4358-4e83-a8ad-e5242bef3240)

### Lab

- Try [this lab test from 2018](https://github.com/skooter500/GE2-Labtest1-2018) about Offset Pursue. No need to clone the repo as it has the solution in it! 

[![YouTube](http://img.youtube.com/vi/bydalDzhCBY/0.jpg)](https://www.youtube.com/watch?v=bydalDzhCBY)

## Week 3

## Lectures
- [Video of Thursdays class about SOLID principals & refactoring](https://web.microsoftstream.com/video/20e70018-e96c-4537-9182-060beefd57a7)
- [Video of Fridays class about Offset Pursue](https://web.microsoftstream.com/video/c14c7cfd-8fa9-407c-be30-e5587f88f487?list=studio)

## Lab

You could use the lab class to work on your assignment - get 3D models imported and flying around or here is an exercise you can do that uses the pursue behaviour we worked on last week: 

Update your fork of the course repo to get the Pursue code we wrote in the class on Friday.

Create a new scene and make this predator prey simulation. The prey will follow a path until the predator comes into range. When the predator is is range the prey will attack the predator by shooting at it. It only shoots at the predator if it is inside the field of view. The predator will get close to the prey, but will flee from the prey if the prey attacks it. You can use colliders and then disable and enable certain behaviours to implement the simulation.

[![YouTube](http://img.youtube.com/vi/SqThPN_ogJE/0.jpg)](https://www.youtube.com/watch?v=SqThPN_ogJE)

To draw the "Lazers" you can use Debug.DrawLine from Update or you could use a LineRenderer

## Week 2 - Path Following, Flee, Pursue & Evade, Banking
- [Video of the class about Player Steering & Pursue](https://web.microsoftstream.com/video/d8be0d36-d9ab-4981-ba33-8d4e20697150?list=studio)

### Part 1 - Path following

Update your fork of the repo with the latest code from the master branch of my repo. To do this, cd to the folder where you have your fork cloned and type:

```bash
git checkout master
git pull upstream master
```

This will get the code we wrote last week. Open the Seek scene and you will see a boid that implements seek and arrive behaviours in the BigBoid.cs class. Today you can implement a path following behaviour for the boid.

Create a branch for your work today:

```bash
git checkout -b lab2
```

Check out this video:

[![Video](http://img.youtube.com/vi/eAfpnWI5jEI/0.jpg)](http://www.youtube.com/watch?v=eAfpnWI5jEI)

The scene contains a game object object with a script called ```Path``` attached. The path script implements the method ```OnDrawGizmos``` to draw lines between the waypoints on the path and to draw a sphere at each of the waypoints. The blue box is following the path. Today you can try and program this behaviour. 

- Implement the ```Path``` script that contains a ```public List<Vector3> waypoints``` containing the waypoints. The 0th waypoint should be the position of the path gameobject itself and the positions of the attached children should be used to set the subsequent waypoints. You can populate this list in ```Awake```. 
- Add a bool flag on the ```Path``` class called ```IsLooped``` to indicate whether the path should loop back to the 0th waypoint when the Boid reaches the last waypoint. If this flag is set to be false, then don't draw a line gizmo back to the 0th waypoint.
- In the scene, create a path using the ```Path``` script you made.
- Add a a public field to the BigBoid class for the Path and drag the Path you made onto this in the Unity editor. 
- Now write code for a behaviour in BigBoid called ```FollowPath``` to get the Boid to move from waypoint to waypoint on the path using Seek and Arrive. If the ```IsLooped``` flag is true on the path, then the Boid should Seek the 0th waypoint again when it reaches the last waypoint. If this flag is set to be false, then the Boid should Arrive at the last waypoint. You will need to add a method called FollowPath and a boolean flag to indicate that the FollowPath behaviour is enabled. 

### Part 2 - Flee

- Implement a behaviour called ```Flee``` that causes the BigBoid to flee from a target when the target comes in range. To do this, add a method called ```Flee``` and a bool flag called ```FleeEnabled``` on the BigBoid class. You will also have to update the ```CalculateForces``` method. Set up your scene with a target game object and move the target around the scene and make sure the Flee force gets activated when the target comes in range.

## Week 1 - Introduction to the course. Introduction to steering behaviours

## Lab
- No lab this week

## Lecture
- [Introduction slides](https://drive.google.com/file/d/1Egwa8jgpLUpQeNJcZ8RuU0Jrt-g65BjU/view?usp=sharing)
- [Steering Behaviours Slides (a bit out of date)](https://drive.google.com/file/d/1nQeVLqhNY1JvAZQK_BgMxUoVr7w1VPUE/view?usp=sharing)
- [Craig Reynolds original paper](https://www.red3d.com/cwr/papers/1999/gdc99steer.pdf)
- [Steering behaviours in Java](https://www.red3d.com/cwr/steer/)