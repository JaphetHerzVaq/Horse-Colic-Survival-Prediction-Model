# Horse-Colic-Survival-Prediction-Model
The purpose of the model is to predict if a horse will survive based upon past medical conditions.

Horse Colic Survival Prediction Model
M.Sc. Japhet Hernández Vaquero
The purpose of the model is to predict if a horse will survive based upon past medical conditions.

Acknowledgements:
The dataset was originally published by the UCI Machine Learning Database http://archive.ics.uci.edu/ml/datasets/Horse+Colic

# Dataset Description
The data contains information on horses' health conditions, treatment course, medical tests (including blood, fecal) and inspections of fluids and gasses.

Surgery: Did the horse was treated with surgery or not?
Age: Age of the horse (adult or young).
Hospital Number: Case Identifier for the horse treated. It may not be unique if the horse received treatment more than once.
Rectal temperature: Measured in Celsius degrees. The normal temperature in horses is 37.8°. An elevated temperature may occur due to an infection. Also, the temperature may be reduced when the animal is in late shock. As illness progresses, this parameter is expected to change (it starts out normal, then it becomes elevated due to the lesion, going back to the normal range as the horse goes into shock.
Pulse: The heart beating frequency rate (in beats per minute). It reflects the heart condition: for adult horses, the normal range is from 30 to 40 beats per minute. It is rare to have lower value, but it is known that athletic horses may have a rate in the range of 20 to 25. Horses with painful lesions or suffering circulatory shock may have an elevated heart rate.
Respiratory rate: The number of breaths the horse takes per minute. The normal rate is 8 to 10.
Temperature of extremities: It is a subjective indication of peripheral circulations (1 - Normal, 2 - Warm, 3 - Cool, 4 - Cold). Cool to cold extremities indicate possible shock. Hot extremities should correlate with an elevated rectal temperature.
Peripheral pulse: It is a subjective variable. Its possible values are: 1 (Normal), 2 (Increased), 3 (Reduced), 4 (Absent). Normal or increased pheripheral pulse are indicative of adequate circulation. Reduced or absent indicate poor perfusion.
Mucous membranes: It is a subjective measurement of colour. Possible values are: 1 (normal pink), 2 (bright pink), 3 (pale pink), 4 (pale cyanotic), 5 (bright red / injected), 6 (dark cyanotic). 1 and 2 probably indicate a normal or slightly increased circulation. 3 may occur in early shock. 4 and 6 are indicative of serious circulatory compromise. 5 is more indicative of a septicemia.
Capillary refill time: It is a clinical judgement. The longer the refill, the poorer the circulation. Its possible values are: 1 (less than 3 seconds) and 2 (more than or equal to 3 seconds).
Pain: It is a subjective judgement of the horse's pain level. Its possible values are: 1 (alert, no pain), 2 (depressed), 3 (intermittent mild pain), 4 (intermittent severe pain), 5 (continuous severe pain). In general, the more painful, the more likely it is to require surgery. Prior treatment of pain may mask the pain level to some extent.
Peristalsis: An indication of the activity in the horse's gut. As the gut becomes more distended or the horse becomes more toxic, the activity decreases. Its possible values are: 1 (hypermotile), 2 (normal), 3 (hypomotile), and 4 (absent).
Abdominal distension: It is considered an important medical parameter. Its possible values are: 1 (None), 2 (slight), 3 (moderate), 4 (severe). An animal that presents abdominal distension is likely to be painful and have reduced gut motility. A horse with severe abdominal distension is likely to require surgery to relieve the pressure.
Nasogastric tube: It refers to any gas coming out of the tube. Its possible values are: 1 (None), 2 (slight), and 3 (significant). A large gas cap in the stomach is likely to give the horse discomfort.
Nasogastric reflux: Net nasogastric reflux is not normal. Occasionally, a small amount of reflux (< 1 L) is obtained if a horse has had an indwelling nasogastric tube. In most adult horses with colic, > 2 L net reflux is abnormal (https://www.msdvetmanual.com/emergency-medicine-and-critical-care/equine-emergency-medicine/equine-emergency-procedures). The possible values are 1 (none), 2 (more than 1 liter) and 3 (less than 1 liter). The greater amount of reflux, the more likelihood that there is some serious obstruction to the fluid passage from the rest of the intestine.
Nasogastric reflux pH: The pH of the reflux. Its scale is from 0 to 14 with 7 being neutral. Normal values are in the range of 3 to 4.
Rectal examination - feces: The presence of feces. Its possible values are: 1 (Normal), 2 (Increased), 3 (Decreased), and 4 (absent). Absent feces probably indicates an obstruction.
Abdomen: Distention in the abdomen. Its possible values are: 1 (Normal), 2 (Other), 3 (firm feces in the large intestine), 4 (distended small intestine), 5 (distended large intestine). 3 is probably an obstruction caused by a mechanical impaction. 4 and 5 indicate a surgical lesion.
Packed cell volume: PCV, a common laboratory test used by equine practitioners. It is the number of red cells by volume in the blood. The normal range is 30 to 50. The level rises as the circulation becomes compromised or as the animal becomes dehydrated.
Total protein: Total plasma protein concentration is a common laboratory test used by equine practitioners. Normal values lie in the range from 6 to 7.5 gms/dL. The higher the value, the greater the dehydration.
Abdominocentesis appearance: Paracentesis of abdomen with content extraction from the peritoneal cavity through punction. A needle is put in the horse's abdomen and fluid is obtained from the abdominal cavity. Its possible values are: 1 (clear), 2 (cloudy), and 3 (serosanguinous). Normal fluid is clear while cloudy or serosanguinous indicates a compromised gut.
Abdominocentesis total protein: Normal abdominal fluid should be straw-colored and clear. A normal protein concentration is less than 2 g/dL. The higher the level of protein, the more likely it is to have a compromised gut.
Outcome: What eventually happened to the horse (1 lived, 2 died, 3 was euthanized).
Surgical lesion: Retrospectively, was the lesion surgical? All cases are either operated upon or autopsied so that this value and the lesion type are always known. Its possible values are: 1 (Yes) and 2 (No).
Type of lesion: There are 3 different columns of this nature. They contain a code formed by 4 different digit codes. The first code number is the type of lesion (1 gastric, 2 sm intestine, 3 lg colon, 4 lg colon an cecum, 5, cecum, 6 transverse colon, 7 rectum/descending colon, 8 uterus, 9 bladder, 11 all intestinal sites, 00 none). The second code number is the type of lesion: 1 (simple), 2 (strangulation), 3 (inflammation), and 4 (other). The third code number is the subtype of lesion: 1 (mechanical), 2 (paralytic) and 0 (not applicable). The fourth code number is an specific code for lesion: 1 (obturation), 2 (intrinsic), 3 (extrinsic), 4 (adynamic), 5 (volvulus/torsion), 6 (intussuption), 7 (thromboembolic), 8 (hernia), 9 (lipoma/slenic incarceration), 10 (displacement) and 0 (n/a)
CP data: Is pathology data present for this case: 1 (Yes) and 2 (No). This variable is of no significance since pathology data is not included or collected for these cases.
