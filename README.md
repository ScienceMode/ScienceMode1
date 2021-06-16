# ScienceMode1

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Device                                                       | RehaStim1                                                    |
| Protocol                                                     | ScienceMode1                                                 |
| Stim. channels                                               | 8                                                            |
| Current (at 1 kΩ load)                                       | 0 – 126 mA (2 mA steps)                                      |
| Pulse width                                                  | 0; 20 – 500 μs (1 μs steps)                                  |
| Frequency                                                    | up to 100 Hz (using all 8 channels); higher rate using lesser channels |
| Pulse shape                                                  | Biphasic pulse                                               |
| Compatibility                                                | ScienceMode1, ScienceMode2 and ScienceMode3 are incompatible |
| Stimulation commands (from PC to the stimulation device)     | 1. Initialize Stimulation: • contains parameters that must be adjusted before start (frequency, activated channels, activated channels with partial frequencies)<br/>• The Stimulator initializes the values and is waiting for the start of the stimulation.<br/>2. Update/Start Stimulation:<br/>• contains parameters pulse width and current; the settings can be adjusted<br/>• The Stimulator starts the stimulation (as start) respectively adapts the transferred parameter (as update).<br/>• enables doublets/triplets (multiple impulses instead of only one)<br/>3. Stop Stimulation:<br/>• The Stimulator stops the Stimulation.<br/>4. Single Impulse:<br/>• contains as parameter one channel, one current and one pulse width.<br/>• The Stimulator has a single output of the impulse with adequate parameters |
| Typical scenario of the commands                             | Initialize, start, update, update, …, stop                   |
| Latency in the execution of stim. commands                   | 2 ms                                                         |
| Electrode error de-tection/feedback                          | Yes/No                                                       |
| Emergency stop availabl./feedback                            | Yes/No                                                       |
| MOTOmed control                                              | No                                                           |
| ScienceMode together with other programs (RehaMove, Sequence Mode) | Yes, but only specific combinations are possible.            |
| C-Library and API                                            | No                                                           |
| Simulink<br/>Control*                                        | There is an open source Simulink-block.<br/>http://sourceforge.net/projects/sciencestim/ |
| Simulink hardware and operation system<br/>support of open source block | • Simulation with Sync-<br/>Block (soft real-time)<br/>Win32/64, Linux32/64<br/>Not yet supported<br/>• Real-Time Windows<br/>Target (hard real-time)<br/>• Eclipse IDE / Embedded<br/>Coder (soft real-time)<br/>not possible<br/>• xPC-Target |

*Simulink is a block diagram environment for multidomain simulation and Model-Based Design. It supports system-level design, simulation, automatic code generation, and continuous test and verification of embedded systems. Simulink provides a graphical editor, customizable block libraries, and solvers for modeling and simulating dynamic systems. It is integrated with MATLAB, enabling you to incorporate MATLAB algorithms into models and export simulation results to MATLAB for further analysis.





