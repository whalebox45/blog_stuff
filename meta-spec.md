*Meta-Spec v2.1*

以下是Spec文件的範本，請依照下列格式撰寫。

----

Spec ID: [SYSTEM]-[MODULE]-[001]

Status: [Draft / Review / Final]

Title: [Title]

Author: [Author name]

Version: [Version ID]

----


## \[專案/功能名稱\]

A standardized specification framework applied to \[請填寫：目標模組或功能的簡短描述\]. Defining exact I/O boundaries and logic before a single line of code is written.

## **1\. Protocol Metadata**

Establishing the fundamental environment, identity, and target scope of this specification document.

### **1.1 Identity & Ownership (META\_TAGS)**

* Spec ID: \[SYSTEM\]-\[MODULE\]-\[001\]  
* Status: \[Draft / Review / Final\]  
* Author: \[Author name\]  
* Version: \[Version ID\]

### **1.2 Scope & Dependencies (ENVIRONMENT)**

* Target: \[e.g., Frontend UI Module / Backend Auth Service / Game Logic\]  
* Framework/Engine: \[e.g., Vue3 / Express.js / Godot 4\]  
* Language: \[e.g., TypeScript / Python / GDScript\]  
* Trigger/Event: \[e.g., HTTP POST / User Click / Audio Sync Hook\]

## **2\. Interface Contract (I/O)**

Defining the explicit boundaries of data entry and side effects. (Crucial: Define this before writing code to prevent hallucination)

### **Inputs**

* \[\[Required/Optional\]\] \[ParameterName\_1\]  
* Type: \[DataType, e.g., string, int, JSON\]  
* Desc: \[詳細描述此輸入數據的作用與邊界限制\]  
* \[\[Required/Optional\]\] \[ParameterName\_2\]  
* Type: \[DataType\]  
* Desc: \[詳細描述此輸入數據的作用與邊界限制\]

### **Outputs**

* \[ReturnType, e.g., JSON, boolean, void\]  
* Desc: \[詳細描述此功能會回傳什麼？或是它僅執行純粹的副作用 (Side-effect)？\]

## **3\. Processing Logic & Algorithm**

\[描述 Inputs 如何被轉換成 Outputs 的完整步驟。若涉及複雜邏輯或數學，請使用 LaTeX 公式或條列式偽代碼。\]

### **Step 1: \[步驟名稱，例如：Data Validation\]**

\[描述該步驟的具體行為，例如：檢查輸入字串是否符合 UUID 格式。\]

### **Step 2: \[步驟名稱，例如：Core Transformation\]**

\[描述核心算法或資料轉換邏輯。例如公式：y \= mx \+ b 或狀態機流轉。\]

### **Step 3: \[步驟名稱，例如：Return / Dispatch\]**

\[描述最終的輸出動作，例如：回傳整理好的 JSON 或觸發特定的 Event 廣播。\]

可以根據步驟的複雜程度來增減步驟。

## **4\. Implementation Constraints (Meta)**

\[此區塊定義 AI 或開發者在實作時必須嚴格遵守的 Coding Style 與架構限制\]

* Typing: \[e.g., 必須使用 TypeScript 嚴格型別，定義 Interface，嚴禁使用 any\]  
* Performance: \[e.g., 必須將結果 Memoize 緩存，時間複雜度不可超過 O(n)\]  
* Paradigm: \[e.g., 強制使用 Functional Programming，禁止修改全域變數\]  
* Naming Convention: \[e.g., 變數使用 camelCase，常數使用 UPPER\_SNAKE\_CASE\]  
* Error Handling: \[e.g., 遇到錯誤時回傳 { success: false, error: "..." } 而非直接 Throw Error\]

可以根據其他需求增減限制。



## **5\. Others**

所有項目的所有e.g.只是範例，不應該只能按照e.g.撰寫，而是視需求設計。

