# Team Vector - Digitalization of narcotics management in an inhouse pharmacy of a veterinary clinic
🐕🐱🐴🐟🦜🦓🦒🦔🦩🦥🦦🐆🐅🦀🦞🐧🦉🦚🦜🐢🐍🦘
 
![doggo](https://github.com/user-attachments/assets/a59f7451-a524-4437-8af4-b7f24fa89b6f)

## Team Members 👨‍💻👩‍⚕️🏥🐾
Firat Turan - firat.turan@students.fhnw.ch 

Giulia Noémie Bleichenbacher - giulianoemie.bleichenbacher@students.fhnw.ch      

Leonie Isele - leonie.isele@students.fhnw.ch      

Sarah Deckarm - sarah.deckarm@students.fhnw.ch      
  


## Coaching 🌟🙏

We would like to thank:


Andreas Martin


Charuta Pande


Devid Montecchiari


For their guidance and support throughout this project. The contributions and insights were truly appreciated.

## Introduction 💊⚠️📄💉❌

Narcotic medications, defined as substances that have a high potential for abuse and are regulated under strict control, fall into a special category of medications in Switzerland, requiring careful management and oversight. 


Narcotic medications are widely used in veterinary medicine. For instance, methadone or buprenorphine may be used to manage severe pain for indications including surgeries, injuries or conditions causing chronic issues. In addition, sedation with, for example, propofol can be used for veterinary patients undergoing certain treatments or surgery, or improved handling or diagnostic procedures. For animals with seizures midazolam may be required. For situations involving euthanasia, certain narcotics, like barbiturates (pentobarbital), are used for compassionate euthanasia in terminally ill or critically injured animals.


The usage of narcotics in a veterinary clinic requires the implementation of rigorous and efficient processes to ensure compliance with regulations and prevent misuse. Experience has shown that the implementation of the processes regarding narcotics management can vary greatly between different clinics. 


Despite legal frameworks, narcotics management is often handled manually with no automation, resulting in inefficiencies and potential risks. For most veterinary clinics, the majority of the process is paper based and is not digitalized. Additionally, there is no clearly defined way of communication between different parties and the responsibility for reordering narcotics out of stock is not specified. In addition, due to disruptions in global supply chains, such as those caused by the COVID-19 pandemic or shipping delays, the availability of critical narcotic medications in veterinary care has been increasingly unpredictable. The lead-up to ordering alternatives is frequently slow, inefficient and occasionally problematic, potentially leading to critical incidents in veterinary care. 


The combination of these issues are truly detrimental to the valuable veterinary healthcare resources and time of, already overworked and understaffed, veterinary staff. A rough estimate has shown that approximately 600h may be spent in an average sized veterinary clinic for managing narcotics with these inefficient processes, with realistic potential spending in the range of 20,000 to 40,000 CHF.  


Our vision is to enhance tracking and streamline workflow management, thereby contributing to the efficiency and safety of narcotic management. Implementing an automated system that suggests alternative medications to supply chain managers, ensuring that any shortages are quickly addressed with minimal disruption allows providing the best possible care for the animal patients. 


## Current Challenges🚩
This problem was addressed in the context of one veterinary clinic, to provide realistic, actionable and viable processes (with possible scaling/generalization to other clinics and/or applications). While this will be described in more detail below, several issues in the current narcotics management are presently highlighted. 

The clinic in question handles all narcotics-related processes manually, with no automation and is exclusively paper based. Stock tracking, repurchasing, and stock updates are all performed manually and are entirely paper-based. This manual documentation leads to inefficiencies and potential human error. 
  
For validation, twice daily, specialized staff counts the number of remaining narcotics, and does a cross validation on the documented usage of narcotics against the remaining stock-- again, all manually and paper-based. This, again, is highly time consuming and does not provide the possibility of flagging inconsistencies automatically. 

In addition, the responsibilities of the different parties are not truly clear, with limited communication between different stakeholders in this process. These ambiguities in accountability and responsibilities may cause critical issues, for instance in delays in reordering narcotics possibly impacting patient care.


## Goal 🎯✨ 
In the context of the previously discussed issues and limitations in the narcotic-related processes in the selected veterinary clinic, we aim to reduce the amount of paperwork by digitalizing the inventory lists and providing an automated reordering process. Thus, human errors can be eliminated, in addition to significantly speeding up the time required for these administrative tasks.

The vision is to ultimately aid in preventing misuse and to increase efficiency for the specialized veterinary staff- allowing a greater focus on patient care. Moreover, the implementation of automated alternative supports the team in providing the optimal and empathetic care that each animal patient requires. 


## AS-IS Process 🔒💊📦🚫📄
 - https://github.com/DigiBP/AS24TeamVector/blob/main/AS-IS_process.bpmn 
   
In the veterinary clinic, there are two safes to store narcotics. The physical location of the safes are very strictly regulated in terms of access, and only limited staff have the rights and possibility to open the safes where the narcotics are stored. A small safe stores the narcotics that can be provided to patients. Additionally, a larger safe, which is only accessible to the team managing narcotics supply, is available to stock up the small safe if needed. This strict dual system provides an additional safe-guard for prevention of narcotics misuse. 



### Narcotics administration 

![AS_IS-subprocess](https://github.com/user-attachments/assets/592747ad-8aee-487c-8e9d-50fb2c4d6e3c)

The as-is process begins with a new patient's arrival, where front staff capture data, followed by the veterinarian's evaluation to determine the new patient's need for narcotics. If they decide that narcotics are required, the sub-process of applying the narcotics to this specific patient is started. The veterinarian fills out a paper form to document the required extensive information on the patient, diverse details on the medication, the indication and the individual indicating/dispensing the medication. After the documentation is completed, subsequently the narcotics are removed and are applied to the patient, ending the process. As a side note, if a new vial is opened but not used up completely, it may be stored for later use for the specific patient it got taken out for. 






### Validation 

![AS_IS-control](https://github.com/user-attachments/assets/ca29fa96-e5cd-418c-80ab-c137268b73af)


To ensure complete correctness, twice a day, one designated veterinarian checks the paper documentation of narcotics used. Then, it is checked against the available stock in the small safe to ensure all entries are valid, there are no discrepancies and everything is tracked correctly. If a discrepancy (deviation) is discovered an investigation is initiated. It is absolutely imperative that any discrepancies are resolved or adequately explained. This process is highly resource-intensive, stressful, and can be frustrating for all parties involved. Failure to resolve this could lead to severe legal implications and limitations in practicing rights, among others.

After the discrepancies are adequately explained, the inventory lists are updated by the narcotics team.





### Inventory and supply chain 

![AS_IS-supply](https://github.com/user-attachments/assets/6e414149-a191-4450-859a-206c955d1864)

Once daily, personnel from the narcotics team checks the big safe's inventory and evaluates with a threshold if an order of new narcotics needs to be placed. The threshold is defined with a great margin to make sure no shortage or delivery difficulties obstruct the availability of the important medications. Thus, it can be ensured that the veterinarians can access important medications directly and easily. 
 
If a narcotic in the small safe falls under a certain threshold it will be restocked from the big safe accordingly manually. Subsequently, the inventory lists are updated by the narcotics team. 

When one or more narcotics in the big safe falls below the threshold, a process to repurchase it will be started. To place the order, the member of the narcotics team, who checked stocks in the big safe, informs the specially trained, qualified purchasing team about the order. The purchasing team then places the order. Contracts/agreements (Verträge zur Beschaffung) for the procurement of these specific medications are often established with authorized suppliers. Upon arrival of the medications, the purchasing team checks the order and accepts it. The narcotics team is informed about the arrival and fills the ordered narcotics into the big safe. Lastly, the staff have to manually update the paper-based inventory list of the big safe again to match the new stock.


### Overview of full AS-IS Process

![AS_IS](https://github.com/user-attachments/assets/3a294fe4-842d-4c2b-be97-37d055706179)






## TO-BE Process 🔍💉🩺📊📦
 - https://github.com/DigiBP/AS24TeamVector/blob/main/TO-BE.bpmn

The to-be process for the supply chain is triggered in a time dependent manner, for instance daily at 11am. Information from the clinic in the form of an inventory list of the small safe is required for this process, and will be explained in further detail below. Additionally, information on the inventory list of the big safe is required. The stocks are kept on a stock list in a csv format, for each safe. 

The number of stocks in both the small and the large small safe are evaluated against a medication-specific threshold to determine if there are sufficient medications available as a service task. So-called “order lists,” or lists containing medications that fall beneath the threshold, are created for each safe. Then, depending on specific conditions, different routes are started. The routes are considered independently for each safe below, and examined in further detail. 


### Route 1: Small safe has insufficient medication stock  transfer from big to small: sufficient narcotics in the big safe 

![Route1](https://github.com/user-attachments/assets/2487498e-8426-453f-a561-38cc462d02e9)

If evaluation of the order list of the small safe determines that a transfer of medications from the big to the small safe is required (i.e. the small safe inventory list shows that one or more medications fall under the required pre-defined threshold), the medications availability is checked in the big safe. If it is available, an order description is created. Personell from the narcotics team is automatically assigned a task with an instruction on the number of medications to transfer. The medications are manually moved from the big to small safe.

Once the narcotics team member confirms that that they transferred the medication from the big to the small safe, this in turn automatically updates both the inventory list of the small and the large safe, with the number of units being removed from the big safe list being added instead to the small safe list. This is implemented as a service task, which calls our API. 


### Route 2: Small safe has insufficient medication stock  transfer from big to small: insufficient narcotics in the big safe
![Route2](https://github.com/user-attachments/assets/fcc3fe77-3d67-48e8-9051-0014b9b87e49)

For robustness, the case when the big safe does not have sufficient medications was considered. This is the case if “is narcotics available” in the big safe is answered with no. Then, the narcotics personell must confirm the shortage, and the order is cancelled. An email notification is sent to the narcotics team, thus ending without updating any of the lists. 

### Route 3: Small safe has sufficient medication stock
![Route3](https://github.com/user-attachments/assets/037861df-d8b8-4a2c-9760-04f17aacc5c5)

If no transfer from the big to small safe is necessary, the small safe process is done here. This is the simplest flow, and will frequently be the case, when narcotic stocks in the small safe are sufficient. 



### Route 4: Big safe has sufficient medication stock
![Route4](https://github.com/user-attachments/assets/69a87111-b4d5-4fc8-92c3-9d177db7b103)

Now, the big safe is described. As previously stated, the order list is created in parallel for both, so also for the big safe. If no narcotic falls below the threshold, no reorder of the big safe required, and the process is done. Again, often the big safe stocks should be sufficient, and this brief process is performed. 


### Route 5: Big safe has insufficient medication stock
![Route5](https://github.com/user-attachments/assets/dba98502-7ee8-493f-8d5c-9b4d5c41284d)


If a narcotic falls below the threshold and a reorder of the medication for the big safe required, the purchasing team is involved. 

A service is implemented (API call, with an internally created API) to check if the medication is available for re-order from the pharmacy (i.e. to check if there are medication shortages on the market currently). Then a Decision Model and Notation (DMN) is implemented, where:

1.	If the medication stock is insufficient but it is available for reorder, the same medication is reordered (typically under the described contracts). 

2.	If the medication is unavailable for order, alternatives are suggested. This includes the name, the ingredient and formulation as well as the producing company, which are based on careful selection by veterinary staff and inbuilt into the logic. Then a manual confirmation is required (i.e. the order would then be sent along with the license - required for the purchase of narcotic medications - per email).   


![Overview](https://github.com/user-attachments/assets/13428d49-cccf-47d5-bc8d-74e9fa223f32)

![DMN](https://github.com/user-attachments/assets/7b029152-336b-440a-9e6b-6346835a6085)

After this decision support in the form of instruction for what to do next, there will be a short latency until the order arrives. Once it has arrived, the purchasing team confirms the order, which then leads to an update in inventory of big safe inventory stock CSV file and an email to the narcotics team. 

### Out of scope processes 

The scope of this project has been adjusted during the course of the collaborative coaching to tackle the ideal processes and to provide the optimal and relevant solutions. To allow for better clarification and as it is not directly relevant for the given process optimization, the veterinarian’s administration process and the narcotic’s team verification process are minimally represented, with focus on only the relevant aspects- and are visualized as “out of the scope”. They are considered as a “customer” of the in-house pharmacy, where the optimization process is performed. 

### Overview of full TO-BE Process 
 ![Screenshot from 2024-12-19 08-43-54](https://github.com/user-attachments/assets/163fe752-840a-4019-9e74-b4d09389c4a7)
![Screenshot from 2024-12-19 08-44-44](https://github.com/user-attachments/assets/f6f2b120-fe74-4df1-b718-76f41989c63e)

Full Overview: 
![Screenshot from 2024-12-19 08-54-12](https://github.com/user-attachments/assets/02f784cb-6d7d-4b2e-ae1f-01292cac6ae4)

## Chatbot/LLM 
-  Please see these links for a brief [explanation](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/Documentation%20-%20Chatbot%20Adventures.pptx) and [video](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/Chatbot_test.mp4) for more information on this sub-project 


### Pilot project  💻👩‍⚕️👨‍⚕️🦠💉🩺🏥🚑🩹
 This is currently seen as a pilot project, with possible implementation on a wider scope. This "to-be" workflow introduces a systematic and automated approach to managing the supply chain for narcotics, with automatic daily triggers and inventory evaluations at predefined thresholds. With the designated routes, complexity in the management is broken down and transferring medications between safes and reordering from external pharmacies when stock is insufficient is made easier. Additionally, addressing scenarios like shortages in the big safe or alternative medication suggestions when reorders are unavailable is crucial. 
 
Expansion to the verification process can be easily imagined and would be an interesting implementation for a future project. While it would bring certain novel complexities (clinical aspects, complexity in administration and data collection), this could likely be nicely digitalized and additionally integrated into the digitalization of the narcotics workflow in a veterinary clinic, with additional value gained. A major advantage in handling the critical tasks of verification and performing calculations to cross-check and flag inconsistencies automatically is that human errors can be eliminated, in addition to streamlining these administrative tasks.


## Conclusions 📦📈💻💊⏳🛠️

The current process (As-Is) for managing narcotics in the veterinary clinic is entirely manual, paper-based, and resource-intensive. Tasks like inventory tracking, validation, and reordering are prone to human error and inefficiencies, with staff spending considerable time on administrative duties instead of patient care. The proposed "to-be" process introduces automation and digitalization, including inventory tracking, threshold-based stock management, and automated reordering workflows. Key improvements include APIs for inventory updates and detection of medication short-passes, decision support systems for alternative medications, and streamlined communication between stakeholders. It solves problems particularily within the scope of the supply chain, and the digitalization of this process helps to both 
enhanced efficiency and reduced paperwork, as well as to minimized errors. This will result in significant savings, as well as better regulatoy/legal compliance and patient care. 
 
![smaller doggo](https://github.com/user-attachments/assets/f774296b-4287-423c-9c50-7c68e3f3fd6e)


## Technologies 🔄⚙️📈📧🛠️

•	Camunda

•	Python 

•	Google Forms 

•	(Voiceflow)


## How to run 📝💻

1.	Start the [link](https://deepnote.com/workspace/Leonie-I-7c59ff99-3227-4911-a84a-ebbab792815e/project/Exercise-Writing-your-own-REST-API-using-Python-Flask-Duplicate-945152e0-66a8-4b9c-b068-364219c8e551/notebook/services-45ceab2ec0ec480bbda50b3c00942923?utm_source=share-modal&utm_medium=product-shared-content&utm_campaign=notebook&utm_content=945152e0-66a8-4b9c-b068-364219c8e551) 
   
2.	Open Camunda Tasklist ([martinlab.science](https://digibp.engine.martinlab.science/camunda/app/tasklist/default/#/?searchQuery=%5B%5D&filter=f0945b62-643a-11ef-8ae6-fa163ee583d0&sorting=%5B%7B%22sortBy%22:%22created%22,%22sortOrder%22:%22desc%22%7D%5D)), username: mi24vector and password: password and follow the processes (see video links below) 

## API Endpoints
1. Retrieve Inventory
- Route: /get_inventory (GET)
- Input parameters: 
    - file_path: file path of either big safe or small safe
- Purpose: Return full inventory list, either of big or small safe, depending on input parameter.
- Action: Reads inventory of big or small save and returns it as a JSON object.
- Response: Full inventory list of specified safe.

2. Update Inventory
- Route: /update_inventory (POST)
- Input parameters: 
    - file_path: file path of either big safe or small safe
    - Name: Name of medication that should be updated
    - operation: add if something should be added to the safe, remove if something should be removed
    - big_safe: True if it is for the big safe, default is false
    - amount: how much should be added or removed
- Purpose: Update big or small safe by removing or adding items
- Action: 
    - Current inventory list is loaded
    - If the operation is 'add', the safe is updated by either the specified amount, or by 2 times the amount that is specified in the inventory list.
    - If the operation is 'remove' either the specified amount or the difference to 0 is removed from the list.
- Response: Full updated inventory list of specified safe.

3. Evaluate Medications
- Route: /evaluate-medications (POST)
- Input parameters: 
    - file_path: file path of either big safe or small safe
- Purpose: Determine what should be reordered for the big safe or what should be restocked in the small safe.
- Action: 
    - Read current Inventory List based on filename
    - Read threshhold based on filename
    - filter items in Inventory list for which the current stock is under the threshold.
- Response: JSON object "orderItem" which contains a list of all narcotics that should be reordered/restocked.

4. Check shortage
- Route: /shortage (POST)
- Input parameters: 
    - narcotic: Name of the narcotic that should be controlled
- Purpose: Simulation of a service that tells you whether there is a shortage for an item or whether it is available for reorder.
- Action: 
    - Check narcotic name for validity
    - Randomly determine whether there is a shortage or not, with a 20% chance of there being a shortage
- Response: JSON containing the following fields:
    - narcotic: name of the narcotic
    - shortage: true or false, depending on whether there is a shortage or not
    - message: "There is (not) currently a shortage of the narcotic"

5. Send E-Mail
- Route: /send-email (POST)
- Input parameters: 
    - to_email: Receiver E-Mail address
    - Subject: subject of the E-Mail message
    - Body: text of the E-Mail message
    - from_email: Sender E-Mail Address
- Purpose: Send an E-Mail
- Action: 
    - Check if all mandatory fields are available
    - Create a MIMEMultipart object, containing the from, to, subject and content of the E-Mail
    - Send E-Mail using smtplib.SMTP and using our team's E-Mail account
- Response: JSON containing either status success or status error 

6. Check refill availability in Big Safe
- Route: /check_refill_availability (POST)
- Input parameters: 
    - orderItem: List of narcotics for which availability should be checked
    - big_safe_file: path of the big safe csv file
- Purpose: Check whether the items that should be restocked in the small safe are available in the big safe.
- Action: 
    - Read big safe inventory and make sure it's valid
    - for each narcotic in orderItem list check that we have twice the amount in the big safe that is specified in the small safe Threshold definition.
    - If that is not the case return the availability and the required amount
- Response: List of all the unavailable narcotics found, including required or available amount, or an empty string if everything is available.   

## Links 🔗

•	[Camunda](https://digibp.engine.martinlab.science/camunda/app/tasklist/default/#/?searchQuery=%5B%5D&filter=f0945b62-643a-11ef-8ae6-fa163ee583d0&sorting=%5B%7B%22sortBy%22:%22created%22,%22sortOrder%22:%22desc%22%7D%5D)

•	[Deepnote](https://deepnote.com/workspace/Leonie-I-7c59ff99-3227-4911-a84a-ebbab792815e/project/Exercise-Writing-your-own-REST-API-using-Python-Flask-Duplicate-945152e0-66a8-4b9c-b068-364219c8e551/notebook/services-45ceab2ec0ec480bbda50b3c00942923?utm_source=share-modal&utm_medium=product-shared-content&utm_campaign=notebook&utm_content=945152e0-66a8-4b9c-b068-364219c8e551) 



Presentation/BPMN 


•	Presentation: https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/Narcovet.pptx


•	BPMN: as is - https://github.com/DigiBP/AS24TeamVector/blob/main/AS-IS_process.bpmn

•	BPMN: to be  - https://github.com/DigiBP/AS24TeamVector/blob/main/TO-BE.bpmn


Videos: 


•	Video – as is process (tokens)  - [video](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/AS%20IS%20Tokens.mp4)

•	Video – to be Route 1-4 (tokens)  - [1](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/Route%201%20tokens.mp4), [2](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/Route%202%20tokens.mp4), [3](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/Route%203%20tokens.mp4), [(4)](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/Route%204%20tokens.mp4), [5](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/Route%205%20tokens.mp4) 

•	Video – Camunda - https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/CamundaScreen-Recording%20(1).mp4

•	Link to example: [CSV changes](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/CSV%20ss.PNG), [Email received](https://github.com/DigiBP/AS24TeamVector/blob/main/presentation%20and%20documentation/Vector_order_arrival.jpeg)   

