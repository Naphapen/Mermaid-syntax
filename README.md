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

⭐**จุดเด่น**
1.ไม่ต้องเสียเวลาจัดเส้นหรือกล่องให้ตรงกัน เพราะระบบจะจัดวาง Layout ให้สวยงามโดยอัตโนมัติ
2.รองรับได้หลายแอปพลิเคชัน เช่น Notion, Obsidian, GitHub, VS Code, และ ChatGPT
3.ป็นตัวอักษร ทำให้สามารถเก็บไว้ใน Git ได้

🛠 **ตัวอย่าง**


graph TD
    %% กำหนดสไตล์ความสวยงาม (เลือกสีกรอบและพื้นหลัง)
    classDef start_end fill:#f9f,stroke:#333,stroke-width:2px;
    classDef process fill:#bbf,stroke:#333,stroke-width:1px;
    classDef decision fill:#f96,stroke:#333,stroke-width:2px;

    %% โครงสร้างของ Flowchart
    Start([เริ่มโปรแกรม]) --> Input[รับค่าคะแนนสอบ]
    Input --> Check{คะแนน >= 50 ?}
    
    %% เส้นทางเงื่อนไข
    Check -- ใช่ --> Pass[แสดงผล: สอบผ่าน 🎉]
    Check -- ไม่ใช่ --> Fail[แสดงผล: สอบตก 📚]
    
    %% จุดจบโปรแกรม
    Pass --> End([จบโปรแกรม])
    Fail --> End

    %% สวมสไตล์ให้กล่องต่าง ๆ
    class Start,End start_end;
    class Input,Pass,Fail process;
    class Check decision;

    <img width="734" height="1361" alt="image" src="https://github.com/user-attachments/assets/924e272e-7c96-4b98-a9c1-6dadf5f1e1fd" />

