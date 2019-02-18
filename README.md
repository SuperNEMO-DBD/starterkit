# SuperNEMO Starter Kit

Documentation and examples for getting started with the SuperNEMO software.

Will initially reuse existing tutorials and examples, maybe use the [LHCb StarterKit](https://lhcb.github.io/starterkit/)
lessons as a template (see also https://github.com/lhcb/starterkit and https://github.com/lhcb/starterkit-lessons)

Here's a list of possible things to include. Might need to be pared down depending on how much time we can get during the meeting itself - we should set priorities.

**Mastering falaise**

- Basic use of Falaise (flsimulate and flreconstruct) - updated version of Ben's Warwick workshop. 
- Standard configurations. For flsimulate, I mean explaining the event generator/vertex combinations for our signal and main backgrounds. For example, when and why we use source_pads_internal vs source_pads, what vertex/event combination corresponds to radon depositing bismuth on tracker wires etc.
- Similarly, we should explain the standard flreconstruct pipeline file, and when and how you might or might not need to configure it.
- To do that we need a basic explanation of databanks and what CAT, track fit etc do, which I think @drbenmorgan already has? Otherwise Cheryl can look at writing slides or something to give a quick explanation.
- We should introduce standard reconstruction modules, by which I mean at least alpha finder and gamma tracking.
- If we have time, I'd like them to run Things2ROOT, PTD2root, & SensitivityModule and see the difference in the outputs. We should also get them running the validation tool, possibly on the standard reconstruction validation module, but see the next point I'm going to make.
- We should get them to make their own module. My suggestion is to use the reconstruction validation module as a starting point (or a pared-down version of it). Reason for this is that it will also teach them how to make an output in the format that the validation tool can understand.

**CCLyon**
- Running falaise software in the singularity container
- Running batch jobs (including sample scripts)
- Where to write to (this might be more a matter of setting policy than sorting out any software stuff)
- What's in MCC2 and how to access it
- Anything we want to say about requesting more official MC

**Commissioning data**
- Where it is on CCLyon
- How to access it (at the moment everyone is working from the CRD files but that shouldn't be the case in the long term, should it?)
- How to interpret it (remembering that many people will not know what a PMT signal looks like, so we could do with a basic intro to the physics).
