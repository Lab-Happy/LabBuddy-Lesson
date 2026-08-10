Folder
[TTL by Function and Number](../../../../500-Resources/510-Datasheets/IC_TTL/TTL_by_Function_and_Number.md)


| Part No. | Description             | Datasheet                                                                                              | DrawIO                                | Circuit                                   | Lesson                               | Lesson ESP32                                   |
| -------- | ----------------------- | ------------------------------------------------------------------------------------------------------ | ------------------------------------- | ----------------------------------------- | ------------------------------------ | ---------------------------------------------- |
| 7400     | Quad 2-input NAND Gate  | [7400](Datasheet/7400_Quadruple_2-Input_Positive-NAND_Gates.pdf)                                       | [7400 drawio](IC_7400_circuit.drawio) | [7400 circuit json](IC_7400_circuit.json) | [7400 Lesson](IC_7400_Lesson.json)   | [7400 Lesson esp32](IC_7400_Lesson_esp32.json) |
| 7402     | Quad 2-input NOR Gate   | [7402](Datasheet/7402_Quadruple_2-Input_Positive-NOR_Gates.pdf)                                        | [7402 drawio](IC_7402_circuit.drawio) | [7402 circuit json](IC_7402_circuit.json) | [7402 Lesson](IC_7402_Lesson.json)   | [7402 Lesson esp32](IC_7402_Lesson_esp32.json) |
| 7404     | Hex Inverter            | [7404](Datasheet/7404_Hex_Inverters.pdf)                                                               | [7404 drawio](IC_7404_circuit.drawio) | [7404 circuit json](IC_7404_circuit.json) | [7404 Lesson](IC_7404_Lesson.json)   | [7404 Lesson esp32](IC_7404_Lesson_esp32.json) |
| 7408     | Quad 2-input AND Gate   | [7408](Datasheet/74HC08.REV1-102589.pdf)                                                               | [7408 drawio](IC_7408_circuit.drawio) | [7408 circuit json](IC_7408_circuit.json) | [7408 circuit](IC_7408_circuit.json) | [7408 Lesson esp32](IC_7408_Lesson_esp32.json) |
| 7411     | Triple 3-input AND Gate | [7411](Datasheet/7411_Triple_3-input_AND_gate.pdf)                                                     | [7411 drawio](IC_7411_circuit.drawio) | [7411 circuit json](IC_7411_circuit.json) | [7411 Lesson](IC_7411_Lesson.json)   | [7411 Lesson esp32](IC_7411_Lesson_esp32.json) |
| 7420     | Dual 4-input NAND Gate  | [7420](Datasheet/7420_Dual_4-input_NAND_gate.pdf)                                                      | [7420 drawio](IC_7420_circuit.drawio) | [7420 circuit json](IC_7420_circuit.json) | [7420 Lesson](IC_7420_Lesson.json)   | [7420 Lesson esp32](IC_7420_Lesson_esp32.json) |
| 7432     | Quad 2-input OR Gate    | [7432](Datasheet/7432__Quadruple_2-Input_OR_Gates.pdf)                                                 | [7432 drawio](IC_7432_circuit.drawio) | [7432 circuit json](IC_7432_circuit.json) | [7432 Lesson](IC_7432_Lesson.json)   | [7432 Lesson esp32](IC_7432_Lesson_esp32.json) |
| 7486     | Quad EXCLUSIVE-OR Gate  | [7486](../../../../500-Resources/510-Datasheets/IC_TTL/Datasheet/7486_Quadruple_2-Input_XOR_Gates.pdf) | [7486 drawio](IC_7486_circuit.drawio) | [7486 circuit json](IC_7486_circuit.json) | [7486 Lesson](IC_7486_Lesson.json)   | [7486 Lesson esp32](IC_7486_Lesson_esp32.json) |
|          |                         |                                                                                                        |                                       |                                           |                                      |                                                |

**วิธีการทดสอบ**
```powershell
PS D:\GitHubRepos\LabBuddy-Firmware\LabBuddy_STM32G431> .\scripts\Test-GateLessonRunner.ps1 -Port COM22 -LessonFile ..\LabBuddy-JC8012P4-HMI\simulator\worksheets\Buffer_8_bit_Lesson_esp32.json

```


| รายการ                                                                                   | ความหมาย                                                |
| ---------------------------------------------------------------------------------------- | ------------------------------------------------------- |
| .\scripts\Test-GateLessonRunner.ps1                                                      | powershell script                                       |
| -Port COM22                                                                              | Serial port ของ LabBuddy worker                         |
| -LessonFile ..\LabBuddy-JC8012P4-HMI\simulator\worksheets\Buffer_8_bit_Lesson_esp32.json | ไฟล์บทเรียนที่จะทดสอบ <br>(ในกรณีนี้เป็น relative path) |
|                                                                                          |                                                         |
