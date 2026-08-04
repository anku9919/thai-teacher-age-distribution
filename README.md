# Thai Teachers Age Structure Analysis
**วิกฤตหรือสมดุล? ถอดโครงสร้างอายุ "ข้าราชการครูไทย" และการกระจายตัวเชิงพื้นที่**

Repository นี้รวบรวมโค้ด Python [Jupyter Notebook วิเคราะห์โครงสร้างอายุครูไทย](https://github.com/anku9919/thai-teacher-age-distribution/blob/main/teacher_age_distribution.ipynb)
ที่ใช้สำหรับการวิเคราะห์เชิงสำรวจ (Exploratory Data Analysis - EDA) 
เพื่อศึกษาโครงสร้างอายุของข้าราชการครูและบุคลากรทางการศึกษา สังกัด สพฐ. ทั่วประเทศไทย 

บทความฉบับเต็มอ่านได้ที่ Medium: [คลิกเพื่ออ่านบทความบน Medium](<ใส่ลิงก์บทความ-Medium-ของคุณที่นี่>)

## 📌 สรุปข้อค้นพบหลัก (Key Findings)
1. **ภาพรวมประเทศดู "สมดุล":** กลุ่มครูจบใหม่ (21-30 ปี) มีจำนวน 162,601 คน ซึ่งใกล้เคียงกับกลุ่มครูใกล้เกษียณ (51-60 ปี) ที่มี 162,235 คน
   ทำให้ในระดับมหภาคดูเหมือนมีอัตรากำลังทดแทนที่เพียงพอ
2. **กำลังหลักคือวัย 31-40 ปี:** คิดเป็นสัดส่วนสูงที่สุดถึง 35.4% ของทั้งระบบ
3. **ความเหลื่อมล้ำเชิงพื้นที่ (Spatial Disparity):** เมื่อนำข้อมูลมาพล็อตลงบนแผนที่ระดับจังหวัด (Choropleth Map)
   พบว่ากลุ่มครูใกล้เกษียณไม่ได้กระจายตัวเท่ากันทั้งประเทศ แต่ไปกระจุกตัวสูงกว่าค่าเฉลี่ยในพื้นที่
   **ภาคอีสานตอนบน-กลาง** และ **ภาคใต้ตอนล่าง** ซึ่งเป็นจุดที่ควรเฝ้าระวังเรื่องการจัดสรรอัตรากำลังในอนาคต

## 📂 แหล่งที่มาของข้อมูล (Data Sources)
* ข้อมูลโครงสร้างอายุข้าราชการครู: ดึงจาก Open Data ของ สพฐ. (OBEC) [dataset_personal/13](https://hrms.obec.go.th/api/opendata/dataset_personal/13)
* ข้อมูลพิกัดและขอบเขตจังหวัดประเทศไทย (GeoJSON): จาก [OpenGISData-Thailand](https://github.com/chingchai/OpenGISData-Thailand)

## 🛠️ เครื่องมือและไลบรารีที่ใช้ (Dependencies)
* `pandas` - สำหรับการจัดการและทำความสะอาดข้อมูล (Data Manipulation)
* `seaborn` / `matplotlib` - สำหรับการสร้าง Data Visualization
* `geopandas` - สำหรับการสร้างแผนที่ (Choropleth Map)

ติดตั้งไลบรารีทั้งหมดได้ผ่านคำสั่ง:
```bash
pip install pandas matplotlib seaborn geopandas
```

หากการวิเคราะห์นี้เป็นประโยชน์ กรุณาอ้างอิงบทความบน Medium และ repository นี้
```
กุลวดี สมบูรณ์วิวัฒน์, [วิกฤตหรือสมดุล? ถอดโครงสร้างอายุข้าราชการครูไทย]. Medium. https://medium.com/@kullawadee/a15b66eb00b4.
Kullawadee Somboonviwat, Thai Teacher Age Distribution EDA [Computer software] GitHub. https://github.com/anku9919/thai-teacher-age-distribution.
```
