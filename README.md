# Team Vector - Digitalization of narcotics management in an inhouse pharmacy of a veterinary clinic
🐕🐱🐴🐟🦜🦓🦒🦔🦩🦥🦦🐆🐅🦀🦞🐧🦉🦚🦜🐢🐍🦘
 
![doggo](https://github.com/user-attachments/assets/a59f7451-a524-4437-8af4-b7f24fa89b6f)


Passwort for Keepass is password

https://deepnote.com/workspace/Leonie-I-7c59ff99-3227-4911-a84a-ebbab792815e/project/Exercise-Writing-your-own-REST-API-using-Python-Flask-Duplicate-945152e0-66a8-4b9c-b068-364219c8e551/notebook/services-45ceab2ec0ec480bbda50b3c00942923?utm_source=share-modal&utm_medium=product-shared-content&utm_campaign=notebook&utm_content=945152e0-66a8-4b9c-b068-364219c8e551

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

The clinic in question handles all narcotics-related processes manually, with no automation and is exclusively paper based. Stock tracking also occurs manually and is paper-based. There is no automation in repurchasing and stock updates. This manual documentation leads to inefficiencies and potential human error. 
  
For validation, twice daily, specialized staff counts the number of remaining narcotics, and does a cross validation on the documented usage of narcotics against the remaining stock-- again, all manually and paper-based. This, again, is highly time consuming and does not provide the possibility of flagging inconsistencies automatically. 

In addition, the responsibilities of the different parties are not truly clear, with limited communication between different stakeholders in this process. These ambiguities in accountability and responsibilities may cause critical issues, for instance in delays in reordering narcotics possibly impacting patient care.


## Goal 🎯✨ 
In the context of the previously discussed issues and limitations in the narcotic-related processes in the selected veterinary clinic, we aim to reduce the amount of paperwork by digitalizing the inventory lists and providing an automated reordering process. A major advantage in handling the critical tasks of checking inventory and performing calculations to cross-check and flag inconsistencies automatically is that human errors can be eliminated, in addition to significantly speeding up the time required for these administrative tasks.

The vision is to ultimately aid in preventing misuse and to increase efficiency for the specialized veterinary staff- allowing a greater focus on patient care. Moreover, the implementation of automated alternative supports the team in providing the optimal and empathetic care that each animal patient requires. 


## AS-IS Process 🔒💊📦
In the veterinary clinic, there are two safes to store narcotics. The physical location of the safes are very strictly regulated in terms of access, and only limited staff have the rights and possibility to open the safes where the narcotics are stored. A small safe stores the narcotics that can be provided to patients. Additionally, a larger safe, which is only accessible to the team managing narcotics supply, is available to stock up the small safe if needed. This strict dual system provides an additional safe-guard for prevention of narcotics misuse. 

# IMG

### Narcotics administration 
The as-is process is initiated with a new patient's arrival and the evaluation performed by the veterinarian to assess the need of narcotics for this individual patient. If they decide that narcotics are required, the sub-process of applying the narcotics to this specific patient is started. The veterinarian fills out a paper form to document the required extensive information on the patient, diverse details on the medication, the indication and the individual indicating/dispensing the medication. After the documentation is completed, subsequently the narcotics are removed and are applied to the patient, ending the process. As a side note, If a new vial is opened but not used up completely, it may be stored for later use for the specific patient it got taken out for. 

# IMG

### Validation 
To ensure complete correctness, twice a day, either staff specifically trained in and assigned to narcotics management or veterinaries check the paper documentation of narcotics used, which is then checked against the available stock in the small safe to ensure all entries are valid, there are no discrepancies and everything is tracked correctly. If a discrepancy is discovered an investigation is initiated. This process is highly resource-intensive, stressful, and can be frustrating for all parties involved. It is absolutely imperative that any discrepancies are resolved or adequately explained, as failure to do so could lead to severe legal implications and limitations in practicing rights, among others.

# IMG

### Inventory and supply chain 
Once daily, personnel from the narcotics team checks the big safes inventory and evaluates with a threshold if an order of new narcotics needs to be placed. The threshold is defined with a great margin to make sure no shortage or delivery difficulties obstruct the availability of the important medications. Thus, it can be ensured that the veterinarians can access important medications directly and easily. If a narcotic in the small safe falls under a certain threshold it will be restocked from the big safe accordingly manually-.
When one or more narcotics in the big safe falls below the threshold, a process to repurchase it will be started. To place the order, the member of the narcotics team, who checked stocks in the big safe, informs the specially trained, qualified purchasing team about the order. The purchasing team then places the order. Contracts or agreements (Verträge zur Beschaffung) for the procurement of these specific medications are often established with authorized suppliers. Upon arrival of the medications, the purchasing team checks the order and accepts it when no discrepancies are present. The narcotics team is informed about the arrival and fills the ordered narcotics into the big safe. Lastly, the staff have to manually update the paper-based inventory list of the big safe again to match the new stock.

# IMG


## Technologies 🔄⚙️📈📧🛠️

•	Camunda

•	Python 

•	Google Forms 

•	(Voiceflow)


🔍📊📝🛑🆘

💉🩺🏥🚑🩹
👩‍⚕️👨‍⚕️🦠


