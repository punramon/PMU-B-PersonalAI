# PMU-B-PersonalAI 🤖
**Class** | **Name** | **Workshop** | **Lecture**
--- | --- | --- | ---
1 | xPore: An AI-Powered App for Bioinformaticians | [Gaussian mixture model](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Workshop_GMM.ipynb) | [Lecture1](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_Xpore%20.pdf)
2 | Learning from Biosignal | [1D CNN for brain signal](https://github.com/punramon/PMU-B-PersonalAI/blob/main/model.py) | [Lecture2](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_learning_from_biosignals.pdf)
3 | AI for detecting code plagiarism | [Code2Vec to detect code clone](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Workshop_CodeCloneDetection.ipynb) | [Lecture3](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_CodeClone.pdf)
4 | Mental disorder detection from social media data | [NLP classifcation](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Workshop_NLPclassifcation.ipynb) | [Lecture4](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_AI%20for%20Detecting%20Users%20with%20Mental%20Disorders%20from%20Social%20media.pdf)
5 | BiTNet: AI for diagnosing ultrasound image | [EffcientNet: Image Classifcaiton](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Workshop_PMUB_Personal_AI_Image_classification_EfficientNetB5.ipynb) | [Lecture5](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_BitNet.pdf)
6 | AI for arresting criminals | [Yolo Detection // Face recognition](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Workshop_Train_Yolov8_Object_Detection_on_Custom_Dataset.ipynb) | [Lecture6](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_ObjectDetection.pdf)

# Content 📝
* [Xpore: An AI-Powered App for Bioinformatics](https://github.com/punramon/PMU-B-PersonalAI/tree/main?tab=readme-ov-file#xpore-an-ai-powered-app-for-bioinformaticians)
* [Learning from Biosignal](https://github.com/punramon/PMU-B-PersonalAI/tree/main?tab=readme-ov-file#learning-from-biosignal)
* [AI for detecting code plagiarism](https://github.com/punramon/PMU-B-PersonalAI/tree/main?tab=readme-ov-file#ai-for-detecting-code-plagiarism)
* [Mental Disorder detection from Social Media Deta](https://github.com/punramon/PMU-B-PersonalAI/tree/main?tab=readme-ov-file#mental-disorder-detection-from-social-media-deta)
* [BitNet: Ai for diagnosing ultrasound image](https://github.com/punramon/PMU-B-PersonalAI/tree/main?tab=readme-ov-file#bitnet-ai-for-diagnosing-ultrasound-image)
* [AI for arresting criminals](https://github.com/punramon/PMU-B-PersonalAI/tree/main?tab=readme-ov-file#ai-for-arresting-criminals)
  
## 📌xPore: An AI-Powered App for Bioinformaticians
**Xpore** เป็นซอฟท์แวร์ที่ช่วยนักชีววิทยาสารสนเทศเปรียบเทียบตำแหน่งของลำดับเบสบนสาย RNA ของเซลล์โดยการใช้ข้อมูลสัญญาณไฟฟ้าที่มาจาก Nanopore Sequencer 

สามารถดูรายละเอียดได้ที่ [Github Xpore](https://github.com/GoekeLab/xpore)

**วัตถุประสงค์**
1. สามารถค้นหาตำแหน่ง m6A บนสาย RNA ได้
2. สามารถทราบ Modification rate (% modified read per total read) ได้
    
**Workshop**

ให้ลองสร้างข้อมูลจาก Data ที่เรา generate ขึ้นมาเอง (โดยเราทราบค่าพารามิเตอร์ต่าง ๆ อยู่เเล้วในกราฟแรก) เพื่อตรวจสอบว่า GMM สามารถหาพารามิเตอร์ได้เท่าไหม 
ซึ่งผลที่ได้กราฟที่เปลี่ยนไปมีการ Shift ไปจากเดิมเนื่องจากค่าเฉลี่ยและส่วนเบี่ยงเบนมาตรฐานเปลี่ยนตามโมเดลของ GMM

## 📌Learning from Biosignal
**TinySleepNet** เป็น Deep learning model ที่ใช้วิเคราะห์การนอนหลับ (ทำนาย stage การนอนหลับโดยใช้คลื่นสัญญาณจากสมอง EEG)

สามารถดูรายละเอียดได้ที่ [Github TinySleepNet](https://github.com/akaraspt/tinysleepnet?fbclid=IwY2xjawG4GSZleHRuA2FlbQIxMAABHaZzuhBKxhjNzvrltT1fQIn2rB_FotzJ6lIkT2cEtUX-ZYeNsBl_qB8nxA_aem_Auik0rZA_9UHruqd77NC3g)

**วัตถุประสงค์**
1. สร้าง Deep learning model ที่มีประสิทธิภาพและสามารถนำไปติดตั้งที่อุปกรณ์ต่าง ๆ เช่นมือถือ หรือ อุปกรณ์ IoT ที่สามารถนำไปวิเคราะห์การนอนของคนไข้ที่อยู่ที่บ้านได้
2. ช่วยลดภาระงานของผู้เชี่ยวชาญและลดเวลาการรอคิวมาตรวจที่โรงพยาบาล
    
**Workshop**

ให้ทำการแก้ไขข้อมูลตรง simple_model ให้ตรงกับ [Model Architecture - Representation Learning](https://github.com/akaraspt/tinysleepnet?tab=readme-ov-file#model-architecture)

## 📌AI for detecting code plagiarism
**Merry** เป็น Machine Learning Model ที่ช่วยตรวจสอบความเหมือนกันของ source code (source code plagiarism detection)

สามารถดูรายละเอียดได้ที่ [Github CodeCloneDetection](https://github.com/MUICT-SERU/SP2019-07-CodeCloneDetection)

**วัตถุประสงค์**
1. เพื่อสร้าง Machine Learning Model ที่สามารถตรวจสอบความเหมือนกันหรือการคัดลอกของ source code ได้อย่างมีประสิทธิภาพ
2. ช่วยลดภาระงานของอาจารย์ที่สอนวิชาเกี่ยวกับการเขียนโปรแกรม และโปรแกรมเมอร์ในการค้นหา source code ที่เหมือนกัน

**Workshop**

ให้ทำการเปรียบเทียบ cosine similarity ในทุก ๆ คู่ของ source code (มีทั้งหมด 16 คู่) --> ค่าเข้าใกล้ 1 หรือเท่ากับ 1 แสดงว่ามีความเหมือนกัน

## 📌Mental Disorder detection from Social Media Data
**AI for Detection User with Mental Disorders from Social media** เป็นการตรวจจับข้อมูลบนสื่อออนไลน์ว่ามีอาการซึมเศร้าหรือไม่ 
โดยจะสกัดข้อมูลจากข้อความ (เช่นจากโพสต์บนสื่ออนไลน์) ว่ามีความรู้สึกอย่างไร เป็น negative หรือ positive แล้วนำไปสร้างโมเดลทำนายต่อไป

สามารถดูรายละเอียดได้ที่ [Researching Mental Health Disorders in the Era of Social Media: Systematic Review](https://www.jmir.org/2017/6/e228/)


**วัตถุประสงค์**
1. เพื่อสร้าง Machine Learning Model ที่ทำนายคนที่เป็นซึมเศร้าโดยข้อมูลบนสื่ออนไลน์อย่างมีประสิทธิภาพ
2. เพื่อที่จะสามารถเข้าช่วยเหลือคนที่เป็นโรคซึมเศร้าหรือเครียดได้

**Workshop**

ให้ทดลองสร้างโมเดล ด้วย Algorithms อื่นๆ ด้วยตัวเอง อีก 2 โมเดล --> Support Vector Classifier และ Random Forest Classifier 

## 📌BitNet: Ai for diagnosing ultrasound image
**BitNet** เป็นระบบที่ช่วยคัดกรองผู้ป่วยมะเร็งท่อน้ำดีโดยการใช้ภาพถ่ายอัลตราซาวด์ 

สามารถดูรายละเอียดได้ที่ [Github BitNet](https://tohnperfect.github.io/BiTNet/)

**วัตถุประสงค์**
1. เพื่อสร้าง model ที่ช่วยคัดกรองผู้ป่วยมะเร็งท่อน้ำดีโดยการใช้ภาพถ่ายอัลตราซาวด์ให้มีประสิทธิภาพ
2. เพื่อช่วยลดภาระงานของรังสีแพทย์และช่วยเพิ่มความมั่นใจในการวินิจฉัยหรือการคัดกรองโรคของแพทย์ GP

**Workshop**

ให้ทดลองนำภาพ นก รถยนต์ เสือ สิงโต และ สุนัขจิ้งจอก มาทำการทำนายและรายงานผลการทำนายแต่ละภาพจากนั้น print output ของ network 

--> ผลทำนายออกมาเป็นสุนัขกับแมวซึ่งไม่ใช่นก รถยนต์ เสือ สิงโต และ สุนัขจิ้งจอกที่เราใส่เข้าไป เนื่องจากข้อมูลที่ใช้เทรนเป็นสุนัขกับแมว (มีแค่ 2 class)


## 📌AI for arresting criminals
**Real-Time Object Detection** ใช้ YOLO ในการทำระบบเฝ้าระวังและบันทึกหลักฐาน พร้อมพัฒนาสู่ระบบแจ้งเตือนด้วยปัญญาประดิษฐ์ เพื่อการตรวจจับและติดตามบุคคลหรือยานพาหนะต้องสงสัย

**วัตถุประสงค์**
1. เพื่อช่วยเจ้าหน้าที่ตำรวจในการจัดเก็บและวิเคราะห์ข้อมูลอาชญากรรมผ่านระบบติดตามผู้ต้องสงสัยด้วยเทคโนโลยีปัญญาประดิษฐ์
2. เพื่อช่วยสร้างความเชื่อมั่นให้กับประชาชนในเรื่องการป้องกันอาชญากรรม

**Workshop**

ให้แยกวิดีโอออกเป็นเฟรมและทำการติด label ให้กับแต่ละเฟรมใน 4 ประเภท ได้แก่ รถบัส, แท็กซี่, รถยนต์, และคนเดินเท้า จากนั้นสร้างโมเดลเพื่อจำแนกประเภททั้ง 4 ด้วย YOLOv8
ซึ่งผลที่ได้จะเห็นว่าทำนาย pedestrian เยอะเกินจริง

ปัญหาอาจเกิดจาก
* Bounding Box อยู่กระจุกซ้อนทับกันเกินไป --> ไม่ชัดเจนแยกไม่ออก
* จำนวน dataset น้องเกินไปทำให้ model มีประสิทธิภาพที่ไม่ดี --> ควรที่จะเพิ่มdataset (extract video เดิมคือ 17 วินาทีได้ 1 เฟรม ซึ่งจะได้ 4 รูป) หรือลดจำนวนวินาทีให้ได้จำนวนภาพที่มากขึ้น


# Presentation video 💿
[![Watch the video](http://img.youtube.com/vi/zEI2lUFZSfg/0.jpg)](https://youtu.be/zEI2lUFZSfg)


