# Project-Prediction-Real-Estate-Price-with-Regression-Model

## การทำนายราคาของอสังหาริมทรัพย์โดยใช้ Regression Model จากภาษา Python 

### สามารถดู Slide Presentation ได้จาก Link: https://www.canva.com/design/DAGQPVPnx-8/OKOX6MfLHC31zYjEb15Ifw/edit?utm_content=DAGQPVPnx-8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton 

สรุปผล: 
จากการ Train Model Regression โดยจะเปรียบเทียบโมเดลระหว่าง Linear Regression และ Ridge Regression ซึ่งเราจะสรุปผลจากค่า RMSE และค่า R-squared ที่ดีที่สุด โดยจะสรุปได้ว่า Ridge Regression ที่มีการจูนค่า alpha = 100 ให้ผลลัพธ์ที่ดีที่สุด

****************************************************

หลังจากหาความรู้เพิ่มเติม(ศึกษาเองผ่านบทความต่าง ๆ)
- dataset ของเราจะมีค่าที่เป็น outlier อยู่ ถ้าเป็นไปได้ควรจะทำ Normalization หรือ Standardization ศึกษาเพิ่มเติมจาก Link: https://www.nerd-data.com/normalization_standardization/
- ควรมีการเทียบโมเดลเพิ่มเติมอย่าง Lasso Regression โดน concept จะมีอยู่ประมาณว่า มันจะทำการตัดตัวแปรนั้นทิ้งไปเลยซึ่งอาจจะเหมาะกับตัวแปรที่มีเยอะๆ และต่างจาก Ridge Regression ที่ทำได้แค่ลดค่าสัมประสิทธิ์ลง แต่จะไม่ใช่การตัดทิ้งไป
- ควรแสดงค่า R-sqaured เพราะ concept คือการลงโทษตัวแปรที่ไม่ส่งผลอย่างเช่น เราทำนายราคารถ(y) ก็จะมีตัวแปรที่เป็น ระยะเดินทาง(x1), บรรจุน้ำมัน(x2), ร้องเพลง(x3) ซึ่งจะตัด x3 ทิ้งแล้วค่า R-squared จะเพิ่มขึ้น เพราะ x3 ไม่ได้เกี่ยวอะไรกับรถเลย
- ควรมีการทำ K-Fold Cross-Validation เปรียบเสมือนกับการจำลองทำข้อสอบเสมือนจริง(Validation Data) ก่อนที่จะลงมือทำจริง(Test Data)
ทั้งหมดนี้เป็นสิ่งที่ผมพอสรุปได้ว่า ตัวเองยังขาดความรู้ในด้านไหนๆบ้าง ซึ่งในการทำครั้งถัดๆไปจะทำให้ดีขึ้นครับ

*****************************************************

ขอบคุณสำหรับคนที่มาอ่านครับ
