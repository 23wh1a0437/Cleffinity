Real Time Project Report
on
“CLEFFINITY”
Submitted in partial fulfillment of the requirements for the award of the degree of
BACHELOR OF TECHNOLOGY
in
ELECTRONICS AND COMMUNICATION ENGINEERING
by
V. PRIYADARSHINI – 23WH1A0435
C. ASHWINI – 23WH1A0437
G. SARANYA – 23WH1A0439
G. TEJASWI – 23WH1A0458
under the guidance of
Mr. R PRIYAKANTH
Department of Electronics and Communication Engineering
BVRIT HYDERABAD College of Engineering for Women
(UGC Autonomous, Approved by AICTE and Affiliated to JNTUH,
Hyderabad) Accredited by NBA and NAAC with A Grade Bachupally,
Hyderabad – 500090
2024-25
DECLARATION
We hereby declare that the work described in this report, entitled “CLEFFINITY”
which is being submitted by us in partial fulfillment for the award of the degree of
Bachelor of Technology in the department of Electronics and Communication
Engineering at BVRIT HYDERABAD College of Engineering for Women (UGC
Autonomous), affiliated to Jawaharlal Nehru Technological University
Hyderabad, Kukatpally, Hyderabad – 500085 is the result of original work carried
out by us under the guidance of Associate professor Mr. R Priyakanth.
This work has not been submitted for any Degree/Diploma of this or any other
institute/university to the best of our knowledge and belief.
Place: Hyderabad
Date:
Names and signatures of the students
V. Priyadarshini -
C. Ashwini -
G. Saranya -
G. Tejaswi -
Department of Electronics and Communication Engineering
BVRIT HYDERABAD College of Engineering for Women
(UGC Autonomous, Approved by AICTE and Affiliated to JNTUH,
Hyderabad) Accredited by NBA and NAAC with A Grade
Bachupally, Hyderabad – 500090
Certificate
This is to certify that the major/mini project report, entitled “CLEFFINITY”
is a record of bonafide work carried out by V.PRIYADARSHINI – 23WH1A0435,
C. ASHWINI – 23WH1A0437, G. SARANYA – 23WH1A0439, G. TEJASWI –
23WH1A0458 in partial fulfillment for the award of the degree of Bachelor of
Technology in the department of Electronics and Communication Engineering at
BVRIT HYDERABAD College of Engineering for Women (UGC
Autonomous), affiliated to Jawaharlal Nehru Technological University
Hyderabad, Kukatpally, Hyderabad – 500085.
Supervisor Head of the Department
ACKNOWLEDGMENT
The satisfaction that accompanies in successful completion of the task would
be incomplete without the mention of the people who made it possible.
We wish to express our deep sense of gratitude to our guide Associate
professor Mr. R Priyakanth, Department of Electronics and Communication
Engineering, BVRIT HYDERABAD College of Engineering for Women, for his able
guidance and suggestions, which helped us in completing this project work on time.
We would like to thank Dr. D. Nagesh, Professor and Head, Department of
Electronics and Communication Engineering for his guidance, support and
encouragement.
We express our gratitude towards our honorable Principal, Dr. K V N Sunitha
and the management for providing all the facilities.
We also thank all the faculty and non-teaching staff members of Electronics and
Communication Engineering department, who supported us directly or indirectly in
successful completion of this project work.
Finally, we thank all our friends and family members for their continuous
support and help.
Names of the students
V. PRIYADARSHINI - 23WH1A0435
C. ASHWINI - 23WH1A0437
G. SARANYA - 23WH1A0439
G. TEJASWI - 23WH1A0458
ABSTRACT
Music education has long relied on visual elements such as written notation
and illustrations, posing significant challenges for individuals who are blind or
visually impaired (VI). Traditional learning materials often fail to address the needs
of these learners, creating barriers to musical literacy and self-expression.
Cleffinity is an innovative and inclusive tool designed to transform how blind
and VI individuals engage with music. By shifting the focus from sight to sound and
touch, Cleffinity enables learners to experience music in a more accessible and
intuitive way. Its multisensory approach fosters independent exploration, allowing
users to connect with musical concepts through tactile feedback and auditory cues.
More than just a learning aid, Cleffinity empowers users to develop confidence
and creativity in their musical journey. It supports self-paced learning and encourages
curiosity, making music education engaging and inclusive, whether in a classroom or
at home. With Cleffinity, music becomes a space where everyone—regardless of
visual ability—can participate, understand, and enjoy.
CONTENTS
1. Introduction Page-1
2. Objectives Page-2
3. System Overview and Methodology
3.1 System Architecture
3.2 Working
3.3 Hardware Components
3.4 Connections
Page-3
4. Features and Innovation Page-6
5. Results and Testing Page-7
6. Conclusion Page-9
7. References Page-10
Appendix Page-12
Final Prototype Page-17
LIST OF FIGURES AND TABLES
Diagram-1 --------------------------------------------------------------------------- page-3
Diagram-2 --------------------------------------------------------------------------- page-5
Diagram-3 --------------------------------------------------------------------------- page-7
Diagram-4 --------------------------------------------------------------------------- page-8
Diagram-5 ---------------------------------------------------------------------------- page-17
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 1
1. Introduction
Music is a universal language that transcends boundaries and connects people
across cultures. However, for individuals who are visually impaired, learning
music can be an immense challenge. Traditional music education heavily
depends on visual aids such as sheet music and diagrams, creating barriers for
those who cannot see. Recognizing this issue, our project "Cleffinity" aims to
provide an accessible and inclusive platform for music education.
Cleffinity is an assistive system that uses a combination of
RFID technology, Braille, raised musical symbols, and audio feedback to help
visually impaired individuals learn and experience music. With this tool,
learners can feel musical notes on the page and hear them simultaneously,
enabling a multisensory learning experience. Our goal is to empower visually
impaired individuals with a self-guided, hands-free, and enjoyable method to
explore music.
The system is designed to function with minimal effort on the part of the user.
Once powered, Cleffinity detects the page being read by sensing the RFID tag
embedded in it. The system instantly retrieves and plays the corresponding
musical note or instruction from the microSD card through a speaker. This
approach eliminates the need for any manual interface, making the device easy
to operate by individuals of all age groups and skill levels. It can also serve as
a foundational platform for more advanced music learning tools, enabling
step-by-step progress for the user.
This project was inspired by the real-world challenges faced by blind learners
who have limited access to musical notation and theory. While there are
existing technologies that support text-to-speech or braille music
transcription, they often require expensive equipment or specialized training.
Cleffinity, in contrast, is affordable, easy to use, and scalable. It utilizes widely
available components and open-source technology, which makes it suitable
for deployment in schools, training centers, or even personal home use.
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 2
2. Objectives
• To develop an accessible system for music learning tailored to visually
impaired users.
• To integrate tactile (Braille and raised symbols) and auditory (sound
playback) feedback.
• To automate music note detection using RFID technology.
• To support multiple instrument tones for better auditory learning.
• To create a user-friendly, interactive, and inclusive learning tool.
• To explore the fusion of embedded systems and inclusive education for
broader societal impact.
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 3
3. System Overview and Methodology
3.1 System Architecture
• RFID tag: Embedded on each page
• RFID reader: Detects tag when page is flipped
• Arduino UNO: Processes tag data and triggers audio
• DFPlayer Mini: Plays MP3 files from SD card
• Speaker: Outputs the note corresponding to the detected tag
3.2 Working
When a user flips a page in the tactile music book, the RFID reader detects the
embedded tag. This information is sent to the Arduino, which retrieves the
corresponding MP3 file from the SD card through the DFPlayer Mini module.
The note is then played aloud, allowing the user to associate the tactile symbol
with the auditory note.
The RFID reader (RC522) operates at 13.56 MHz and communicates with the
Arduino UNO via the SPI protocol. Each RFID tag is programmed with a
unique identifier, which is linked to an audio file. The DFPlayer Mini is a
compact MP3 module with an inbuilt amplifier, making it ideal for portable
applications. The use of raised tactile symbols printed or embossed onto the
music sheet helps the user trace and identify note positions. The integration of
both touch and sound significantly enhances learning efficiency.
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 4
Diagram-1 (Block Diagram)
3.3 Hardware Components
• Arduino UNO: Microcontroller board for system control
• RFID Reader (RC522): Reads the RFID tag from the music page
• RFID Tags (stickers): Embedded in each page to encode unique audio
instructions
• DFPlayer Mini MP3 Module: Retrieves and plays MP3 files from a
microSD card
• Speaker: Converts electrical signals into audio output
• Micro SD Card with MP3 audio files: Stores audio samples for notes
and tones
• Braille-enabled and raised symbol music pages: Provide tactile
feedback to users
Audio files are recorded in high quality to ensure clarity and distinctiveness
of each note.
3.4 Connections
1. RFID RC522 to Arduino
RFID RC522 Pin Arduino Pin
SDA (SS) 10
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 5
SCK 13
MOSI 11
MISO 12
GND GND
RST 9
3.3V 3.3V
2. DF Mini MP3 Player to Arduino
DF Mini MP3 Player Pin Arduino Pin
VCC 5V
GND GND
RX D6
TX D5
SPK1 Speaker (+)
SPK2 Speaker (−)
Diagram-2 (Circuit Diagram)
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 6
4. Features and Innovation
• Touch and Sound Integration: Users feel notes with their fingers and
hear them simultaneously creating a powerful multisensory experience.
• Multiple Instrument Sounds: Each note is available in different
instrument tones such as piano, violin, and guitar. This enhances
auditory memory and improves the ability to differentiate sounds.
• Hands-Free Operation: The device activates automatically upon page
flip, without any need for buttons or screen interaction.
• Inclusive Learning: Designed to be used by individuals with no prior
exposure to music, ensuring accessibility for beginners and children.
• Scalable and Customizable: Can be adapted to various educational
content beyond music, including alphabets, stories, and general
knowledge.
• Affordable and Open-Source: Built using low-cost components and
open-source tools to encourage widespread adoption.
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 7
5. Results and Testing
The Cleffinity prototype was assembled and tested in a controlled setting to
verify the functionality of each component. The RFID module successfully
detected tags placed on different pages, and the DFPlayer Mini module
responded by playing the correct corresponding audio file for each tag.
All components—Arduino, RFID reader, speaker, and DFPlayer—worked in
coordination to produce a smooth and consistent experience. The sound output
was clear, and each tag triggered the expected audio file without errors. The
system showed good responsiveness, with minimal delay between scanning a
tag and hearing the audio.
The audio files were played through a speaker connected to a direct power
source, ensuring consistent performance throughout testing. The logic for
matching specific tags to particular audio files functioned as intended,
confirming the accuracy of the software-hardware integration.
This successful test demonstrates that Cleffinity is technically functional and
ready for further improvements or real-world application trials.
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 8
Diagram-3 (Connections)
Diagram-4 (Total setup)
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 9
6. Conclusion
Cleffinity presents a step forward in inclusive education technology. By
combining tactile and auditory feedback, it breaks down the barriers of
traditional music learning for visually impaired individuals. The project
showcases how embedded systems, when integrated thoughtfully, can
transform education and accessibility.
The simplicity of Cleffinity allows for mass production and wide adoption. Its
modularity means it can be adapted to include more complex musical pieces
or even theoretical lessons in future versions. Additional features like
Bluetooth connectivity, app integration, or quiz modes could further enhance
the learning experience.
Future enhancements may include Bluetooth headphones, interactive quizzes,
and support for music theory education. Overall, Cleffinity is not just a
project—it’s a movement toward making music truly for everyone.
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 10
7. References
Journals:
[1] J. A. Borges and D. Tomé, “Teaching music to blind children: New strategies
for teaching through interactive use of musibraille software,” Procedia Comput.
Sci., vol. 27, pp. 19–27, 2014.
[2] L. Lu, K. A. Cochrane, J. Kang, and A. Girouard, “‘Why are there so many
steps?’: Improving Access to Blind and Low Vision Music Learning through
Personal Adaptations and Future Design Ideas,” ACM Trans. Access. Comput.,
vol. 16, no. 2, pp. 1–20, 2023.
[3] N. F. Tisnawati, Yuliati, and E. Purbaningrum, “Braille innovation technology
in teaching and learning process for visual impairment,” JTP - J. Teknol.
Pendidik., vol. 24, no. 2, pp. 224–235, 2022.
Weblinks:
1. Arduino Documentation
https://www.arduino.cc/en/Guide/HomePage
For understanding Arduino programming, board connections, and hardware
interfacing.
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 11
2. MFRC522 RFID Reader Library
https://github.com/miguelbalboa/rfid
For using the MFRC522 RFID module with Arduino.
3. DFPlayer Mini MP3 Player Library
https://github.com/DFRobot/DFRobotDFPlayerMini
For interfacing DFPlayer Mini and playing audio files through Arduino.
4. DFRobot Wiki - DFPlayer Mini
https://wiki.dfrobot.com/DFPlayer_Mini_SKU_DFR0299
Technical documentation and example usage for the DFPlayer Mini module.
5. Braille Music Notation Reference
https://www.loc.gov/nls/music/
https://library.tsbvi.edu/assoc_files/92120013_1.pdf
Understanding how Braille is used for music education.
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 12
Appendix
Code:
#include <SPI.h>
#include <MFRC522.h>
#include <SoftwareSerial.h>p
#include <DFRobotDFPlayerMini.h>
#define SS_PIN 9
#define RST_PIN 8
#define DF_RX 6
#define DF_TX 7
MFRC522 rfid(SS_PIN, RST_PIN);
SoftwareSerial mySerial(DF_RX, DF_TX);
DFRobotDFPlayerMini myDFPlayer;
// Store 8 RFID tags and their assigned audio files
String tagList[8] = {
"1d61baa4b1080", // Tag 1 -> 0001.mp3
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 13
"1d62baa4b1080", // Tag 2 -> 0002.mp3 "1d63baa4b1080", //
Tag 3 -> 0003.mp3
"1d64baa4b1080", // Tag 4 -> 0004.mp3
"1d65baa4b1080", // Tag 5 -> 0005.mp3
"1d66baa4b1080", // Tag 6 -> 0006.mp3
"1d67baa4b1080", // Tag 7 -> 0007.mp3
"1d68baa4b1080" // Tag 8 -> 0008.mp3
};
void setup() {
Serial.begin(9600);
SPI.begin();
rfid.PCD_Init();
Serial.println("RFID Ready!");
mySerial.begin(9600);
Serial.println("Initializing DFPlayer...");
if (!myDFPlayer.begin(mySerial)) {
Serial.println("DFPlayer Mini NOT detected! Check wiring.");
while (true);
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 14
}
Serial.println("DFPlayer Mini is working!");
myDFPlayer.volume(15); // Set volume (0-30)
}
void loop() {
if (!rfid.PICC_IsNewCardPresent()) return;
if (!rfid.PICC_ReadCardSerial()) return;
// Read the card UID
String cardID = "";
for (byte i = 0; i < rfid.uid.size; i++) {
cardID += String(rfid.uid.uidByte[i], HEX);
}
Serial.print("Scanned Tag UID: ");
Serial.println(cardID);
// Check if the tag matches one of the 8 stored UIDs
int assignedFile = -1;
for (int i = 0; i < 8; i++) {
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 15
if (cardID == tagList[i]) {
assignedFile = i + 1; // Assigns file 0001.mp3 to 0008.mp3
break;
}
}
if (assignedFile != -1) {
Serial.print("Playing Audio File ");
Serial.println(assignedFile);
myDFPlayer.play(assignedFile);
} else {
Serial.println("Unknown Tag! No audio played.");
}
delay(4000); // Wait before allowing another scan
rfid.PICC_HaltA();
}
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 16
Cleffinity
Department of ECE, BVRIT HYDERABAD CEW Page 17
Final Prototype
