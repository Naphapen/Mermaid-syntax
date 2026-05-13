# Mermaid-syntax
What is Mermaid syntax

Mermaid syntax คือ ภาษาที่ใช้ในการสร้างแผนภูมิ (Diagram) และกราฟต่าง ๆ โดยใช้ Text-based code (การพิมพ์ตัวอักษร) แทนการลากวางผ่านโปรแกรมวาดรูป

🛠 **ทำงานอย่างไร?**
หลักการของมันคือการใช้สัญลักษณ์ง่าย ๆ เพื่อบอกความสัมพันธ์ เช่น หากต้องการบอกว่า A ไปหา B เราจะพิมพ์
A --> B

*ตัวอย่าง*
graph TD
    A[เริ่มโจทย์] --> B{ตัดสินใจ}
    B -- ใช่ --> C[ไปต่อ]
    B -- ไม่ใช่ --> D[จบการทำงาน]

Mermaid มีความสามารถหลากหลายมาก โดยรองรับการสร้างแผนภูมิหลายประเภท
1.Flowcharts
2.Sequence Diagrams
3.Gantt Charts
4.Class Diagrams & Entity Relationship (ER)
5.Mind Maps & User Journeys
