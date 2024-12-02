# PMU-B-PersonalAI 🤖
**Class** | **Name** | **Workshop** | **Lecture**
--- | --- | --- | ---
1 | xPore: An AI-Powered App for Bioinformaticians | [Gaussian mixture model](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Workshop_GMM.ipynb) | [Lecture1](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_Xpore%20.pdf)
2 | Learning from Biosignal | 1D CNN for brain signal | [Lecture2](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_learning_from_biosignals.pdf)
3 | AI for detecting code plagiarism | [Code2Vec to detect code clone](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Workshop_CodeCloneDetection.ipynb) | [Lecture3](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_CodeClone.pdf)
4 | Mental disorder detection from social media data | NLP classifcation | [Lecture4](https://github.com/punramon/PMU-B-PersonalAI/blob/main/Lecture/Lecture_AI%20for%20Detecting%20Users%20with%20Mental%20Disorders%20from%20Social%20media.pdf)
5 | BiTNet: AI for diagnosing ultrasound image | EffcientNet: Image Classifcaiton | Lecture5
6 | AI for arresting criminals | Yolo Detection // Face recognition | Lecture6

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

## 📌Mental Disorder detection from Social Media Deta
**AI for Detection User with Mental Disorders from Social media** เป็นการตรวจจับข้อมูลบนสื่อออนไลน์ว่ามีอาการซึมเศร้าหรือไม่ 
โดยจะสกัดข้อมูลจากข้อความ (เช่นจากโพสต์บนสื่ออนไลน์) ว่ามีความรู้สึกอย่างไร เป็น negative หรือ positive แล้วนำไปสร้างโมเดลทำนายต่อไป

สามารถดูรายละเอียดได้ที่ [Researching Mental Health Disorders in the Era of Social Media: Systematic Review](https://www.jmir.org/2017/6/e228/)


**วัตถุประสงค์**
1. เพื่อสร้าง Machine Learning Model ที่ทำนายคนที่เป็นซึมเศร้าโดยข้อมูลบนสื่ออนไลน์อย่างมีประสิทธิภาพ
2. เพื่อที่จะสามารถเข้าช่วยเหลือคนที่เป็นโรคซึมเศร้าหรือเครียดได้

**Workshop**

## 📌BitNet: Ai for diagnosing ultrasound image

## 📌AI for arresting criminals

# Presentation video 💿
