# QT 視窗程式作業(Client & Server傳輸)

## 內容
---

#### 使用者可以指定要傳送的網址及port

---

## 說明
---

#### 我創建2個QLineEdit一個輸入網址一個輸入port，當使用者按下開始時，程式會讀取當前的url及port，並傳輸到該url:port

---

## 結果

#### 1. Clinet指定url: 127.0.0.1 port: 16998 | Server監聽於: url:127.0.0.1:16998
![測試1](/doc/測試1.png)
#### 結果1:可以正常傳輸

#### 2. Clinet指定url: 127.0.0.1 port: 6555 | Server監聽於: url:127.0.0.1:16998
![測試2](/doc/測試2.png)
#### 結果2: 因為監聽port不同，所以無法傳輸

#### 3. Clinet指定url: 127.0.0.1 port: 6555 | Server監聽於: url:127.0.0.1:6555
![測試3](/doc/測試3.png)
#### 結果3: 我把Server 監聽port改成6555就可以傳輸

#### 4. Clinet指定url: 127.0.1.1 port: 6555 | Server監聽於: url:127.0.0.1:6555
![測試4](/doc/測試4.png)
#### 結果3: 因為url跟server不同，所以無法run

---
##### By. wenwen

##### 參考資料:
[nckugs(TcpFileSender)](https://github.com/nckugs/TcpFileSender)
[nckugs(TcpFileServer)](https://github.com/nckugs/TcpFileServer)