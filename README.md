My name is Pierre F. Maldague. I am a scientist and software engineer, with a lot of experience in Space Mission planning and scheduling. My original goal in life was to elucidate the mathematical difficulties that plague quantum field theory, but that turned out to take a lot longer than anticipated. In the meantime, I did useful things for NASA/JPL as a software programmer. With my colleagues (mostly Adans Ko and Steve Wissler) I developed an incredible application called APGen or, in its latest incarnation for the Europa Clipper mission, APGenX. Over the years, APGen has allowed mission engineers to identify countless problems in preliminary spacecraft design. It has also helped space missions save considerable cost by automating Mission Operations tasks. See the paper by Steve Wissler et al. and by Eric Ferguson et al. in the Proceedings of the 2014 and 2018 SpaceOps Conferences for illuminating examples of what APGen has been able to accomplish.

The open-apgen repository contains the source code for the APGen application, which has been open-sourced by JPL-CalTech in 2021. The code has been refactored many times, mostly by me since my requests for programming help went unanswered for many years. The documentation leaves much to be desired, and the program is not easy to use. This being said, it will do wonders for you - especially if you happen to be in charge of a billion dollar-plus space mission with a complex spacecraft and a projected life span of many years.

At the core of APGen, there is a Domain-Specific Language (DSL) which resembles C in its arithmetic capabilities. The DSL is not meant as a replacement of established languages such as C or Java. The people using APGen are called "adapters". An adapter is an engineer, usually not a programmer, who is familiar with the spacecraft and/or the behavior of its subsystems. Because the DSL is simpler than C, the initial learning curve is easy to climb. Where the DSL turns both powerful and interesting is in its ability to express both the structure and the behavior of a complex system in a manner that is flexible, concise and "tweakable". The most productive use of APGen has taken place during design and implementation phases of a mission, when requirements are evolving on a monthly basis and design tradeoffs need to be made constantly. APGen's tweakability has been an essential reason for its success.

APGen can also be used to automate the operation of complex spacecrafts, once the mission has reached its operational phase. APGen is currently used in this way by a number of NASA space missions, including Juno and InSight. The key rôle of APGen, when used in this mode, is to create an activity plan subject to constraints. The constraints can reflect timing or resource consumption requirements. The DSL can be used to express more complex requirements such as priority-based filtering of tentative schedules of conflicting activities. Scheduling runs are usually followed by a comprehensive simulation run that validates the entire plan. On the Europa Clipper mission, APGen routinely performs such simulations between 5,000 and 10,000 times faster than real-time.
For more information, please consult [my résumé](./PFMResume.pdf), a copy of which can be found in this repository.
