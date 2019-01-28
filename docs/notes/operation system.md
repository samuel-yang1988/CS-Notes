* [一、概觀](#概觀)
    * [1.什麼是作業系統?](#什麼是作業系統?)
    * [2.作業系統定義](#作業系統定義)
    * [3.作業系統元件](#作業系統元件)
    * [3.作業系統基本服務](#作業系統基本服務)
* [二、行程(process)和行程管理](#行程(process)和行程管理)  
# 一、概觀

## 1.什麼是作業系統?
   *  介於軟體和硬體中間
   *  隱藏硬體的複雜性(讀/寫檔案系統、傳送接收網路封包)
   *  處理資源管理 (CPU調度、記憶體管理)
   *  提供隔離和保護(將不同部分記憶體分配給不同的應用程式，以便應用程式不會覆蓋其他記憶體。)
## 2.作業系統定義
     作業系統是一層系統軟體
   *  直接擁有特權對底層元件存取的權限
   *  隱藏硬體的複雜度;
   *  根據一些預先定義的策略代表一個或多個應用程式管理硬體
   *  此外他還可以確保應用程式彼此獨立並被保護
## 3.作業系統元件
   *  抽象(對應於OS執行的應用程序)
      * process,thread,file,socket,memory page
   *  機制(在抽象之上)
      * create,schedule,open,write,allocate
   *  策略(如何使用機制管理底層的硬體)
      * Least Recently Used (LRU) , Earliest Deadline First (EDF), etc.
## 4. 作業系統基本服務
   * process management
   * file management
   * device management
   * memory management
   * storage management
   * security

# 二、行程(process)和行程管理
## 行程(process)：實例化於一個運行的程式(Program)
   * 執行狀態(Sate)
      * program counter、stack pointer
   * Parts and Temporary Holding Area 
      * data, register state, occupies state in memory
   * May require special hardware
      * I/O devices
   * Process is a state of a program when executing and loaded in memory (active state) as opposed to application (static state).
   

