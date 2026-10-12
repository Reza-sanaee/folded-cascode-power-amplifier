# Analog Power Amplifier: Complete Assignment

## Objective and supplied circuit

Following the earlier LM741 investigation, design a differential high-gain amplifier and output stage capable of driving a 100-ohm load. Apply feedback to obtain the specified closed-loop gain. Start from the supplied circuit diagram, analyze especially the output stage, identify its limitations, and modify it to meet the design targets. Replace independent sources other than the positive and negative supply rails with appropriate circuits.

## Initial analysis: ten required tasks

1. Identify input and output stages.
2. Explain Q6 and the bias-current source IB; choose IB so Q5 remains on.
3. Calculate transistor operating points and tabulate them.
4. Explain the dead zone expected from class-B output without feedback and how feedback reduces its effect.
5. Calculate output swing and input common-mode range.
6. Identify the mechanisms limiting swing.
7. Simulate in LTspice and show the circuit.
8. Observe node X and the output, comparing the waveforms with the dead-zone analysis.
9. Adjust operating points to increase swing and report the maximum simulated waveform.
10. Define total harmonic distortion and determine it from the simulation.

## Targets and permitted devices

| Requirement | Target |
|---|---|
| Output swing | Greater than 16.6 V peak-to-peak |
| THD | Below 0.05 percent at 16.4 V peak-to-peak |
| Closed-loop gain | 2 |
| Rest/quiescent power | At most 50 mW |
| Supplies | +10 V and -10 V |
| Transistor count | Fewer than 25 |

Use 2N3906-derived PNP transistors with bf=150 and 2N3904-derived NPN transistors with bf=200, through the specified LTspice model overrides. Only one output-stage transistor may use a different chosen saturation-current parameter while otherwise retaining the permitted model properties.

## Redesign tasks

Draw a folded-cascode input stage, explain its advantages and operating-point selection, and replace the original input with it. Replace all nonsupply sources. In the output stage, replace only current sources with suitable current mirrors; additional output-stage changes are prohibited. Input-stage and interstage-level adjustments are allowed. Simulate and show the redesigned circuit. Provide separate evidence for closed-loop gain, output swing, no-input power, and THD at symmetric +/-8.2-V output. Repeat with the assignment's specified larger feedback resistors and show the output; optionally explain the resulting distortion.

## Report and files

Number all figures and tables and cite them in the text. Put figure captions beneath figures and table captions above tables. Include every necessary plot and a full explanation because the report is the grading basis. Work individually. Submit distinct, meaningful filenames for the report and simulation files in an organized ZIP. When design freedom is substantial, state reasonable assumptions and justify choices. Preserve the supplied schematic, operating-point requirements, and target table.
