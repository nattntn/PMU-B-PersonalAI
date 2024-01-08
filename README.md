# PMU-B-PersonalAI :space_invader:
# VDO PRESENTATION :octocat:
# CONTENTS :octocat:

|  ᴄʟᴀꜱꜱ   |                     ɴᴀᴍᴇ                        |  ᴡᴏʀᴋꜱʜᴏᴘ     | ʟᴇᴄᴛᴜʀᴇ  |ᴅᴏᴄᴜᴍᴇɴᴛ  |
|:-------:|:-----------------------------------------------:|:-------------:|:--------:|:---------:|
|   1     | xᴘᴏʀᴇ: ᴀɴ ᴀɪ-ᴘᴏᴡᴇʀᴇᴅ ᴀᴘᴘ ꜰᴏʀ ʙɪᴏɪɴꜰᴏʀᴍᴀᴛɪᴄꜱ      | [ɢᴀᴜꜱꜱɪᴀɴ ᴍɪxᴛᴜʀᴇ ᴍᴏᴅᴇʟ](xPore/GMM.ipynb) | Test1 |   [:paperclips:](https://drive.google.com/drive/folders/1WzSEFgym7sDo-3A9etN1a210a0IYmDi_),[:cd:](https://powerclass.org/courses/xpore-an-ai-powered-app-for-bioinformaticians/)      |
|   2     | ʟᴇᴀʀɴɪɴɢ ꜰʀᴏᴍ ʙɪᴏꜱɪɢɴᴀʟ                          |[1ᴅ ᴄɴɴ ꜰᴏʀ ʙʀᴀɪɴ ꜱɪɢɴᴀʟ](Biosignal/model.py) | Test2 | 111|
|   3     | ᴀɪ ꜰᴏʀ ᴅᴇᴛᴇᴄᴛɪɴɢ ᴄᴏᴅᴇ ᴘʟᴀɢɪᴀʀɪꜱᴍ                 | [ᴄᴏᴅᴇ2ᴠᴇᴄ ᴛᴏ ᴅᴇᴛᴇᴄᴛ ᴄᴏᴅᴇ ᴄʟᴏɴᴇ](CodeClone/PMU_B_CodingAI_CodeCloneDetection_Workshop.ipynb) | Test3 |111|
|   4     | ᴍᴇɴᴛᴀʟ ᴅɪꜱᴏʀᴅᴇʀ ᴅᴇᴛᴇᴄᴛɪᴏɴ ꜰʀᴏᴍ ꜱᴏᴄɪᴀʟ ᴍᴇᴅɪᴀ ᴅᴀᴛᴀ | [ɴʟᴘ ᴄʟᴀꜱꜱɪꜰɪᴄᴀᴛɪᴏɴ](NLP_classification/PMU_B_CodingAI_NLP_classification_Workshop_ipynb.ipynb) | Test1 |111|
|   5     | ʙɪᴛɴᴇᴛ: ᴀɪ ꜰᴏʀ ᴅɪᴀɢɴᴏꜱɪɴɢ ᴜʟᴛʀᴀꜱᴏᴜɴᴅ ɪᴍᴀɢᴇ       | [ᴇꜰꜰᴄɪᴇɴᴛɴᴇᴛ: ɪᴍᴀɢᴇ ᴄʟᴀꜱꜱɪꜰɪᴄᴀɪᴛᴏɴ](BiTNet/PMUB_Personal_AI_Image_classification_EfficientNetB5.ipynb) | Test2 |111|
|   6     | ᴀɪ ꜰᴏʀ ᴀʀʀᴇꜱᴛɪɴɢ ᴄʀɪᴍɪɴᴀʟꜱ                       | [ʏᴏʟᴏ ᴅᴇᴛᴇᴄᴛɪᴏɴ // ꜰᴀᴄᴇ ʀᴇᴄᴏɢɴɪᴛɪᴏɴ](Detection/PMU_B_Train_Yolov8_Object_Detection_on_Custom_Dataset_Workshop.ipynb) | Test3 |111|

   ## :pushpin: ᴄʟᴀꜱꜱ 1 : xᴘᴏʀᴇ: ᴀɴ ᴀɪ-ᴘᴏᴡᴇʀᴇᴅ ᴀᴘᴘ ꜰᴏʀ ʙɪᴏɪɴꜰᴏʀᴍᴀᴛɪᴄꜱ 
>**xPore** คือ แอปพลิเคชันที่เอาไว้หาตำแหน่งของ RNA modification(m6A) ซึ่งพัฒนาโดยใช้ Machine Learning ผ่านชุดข้อมูลที่ได้มาจากเครื่องมือ Nanopore Sequencing เพื่อมาทำความเข้าใจสัญญาณไฟฟ้าที่ได้ และนำมาเปรียบเทียบสัญญาณไฟฟ้าระหว่างคนที่ปกติ กับคนที่เป็นโรค 
   * **ที่มาและความสำคัญ**
     
     เนื่องจากว่าการแสดงออกของ Gene (Gene Expression) :dna: เป็นสิ่งที่สำคัญ หากมีการทำงานที่ผิดปกติไปจากเดิม อาจเป็นเหตุผลให้เกิดโรคขึ้นภายในร่างกายของเราได้ ซึ่งเป็นสาเหตุที่ทำให้เราต้องทราบว่า DAN/mRNA/Protein มีการทำงานผิดปกติจากเดิมอย่างไร โดยการนำ mRNA ไปทำ Sequencing เพื่อดูความผิดปกติของสาย mRNA ซึ่งวิธีเดิมจะต้องทำการแปลง mRNA กลับไปเป็น DNA ก่อน ซึ่งจะเรียกว่า cDNA ซึ่งกระบวนการนี้จะทำให้เราไม่สามารถ Detect ดูลำดับบเบสได้โดยตรง จึงได้มีการพัฒนา **xPore**ขึ้นมา ซึ่ง xpore เป็น direct RNA sequencing จึงไม่ต้องทำการแปลงRNA กลับไปเป็น DAN ทำให้ **ถ้าหากมีอะไรผิดปกติในลำดับเบสเราจะสามารถ detect ได้เลย อีกทั้งตัวเครื่องยังมีขนาดเล็ก พกพาสะดวก ใช้งานง่าย และมีความรวดเร็วในการทำงาน**
   * **วัตถุประสงค์**
     1. เพื่อให้ทราบว่ามี m6A อยู่ที่ตำแหน่งไหนบนสาย RNA
     2. เพื่อให้ทราบว่ามีกี่ % ของจำนวน Read ที่ได้มีการ Modified ไป (ทำ Modification rate เพื่อดูว่าเกี่ยวข้องยังไงกับการทำงานของร่างการ(ปกติ/เป็นโรค))
   
