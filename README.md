# 데이터처리언어 Fraud Detection Project EDA


## 📃 Data
 **[IEEE CIS Fraud Detection Dataset](https://www.kaggle.com/competitions/ieee-fraud-detection)**


```bash
# User data
TransactionID | Id_1~Id_38 | DeviceType | DeviceInfo

# Transaction data
TransactionID | isFraud | TransactionDT | TransactionAMT | ProductCD | card1~6 | Addr1,2 | Dist1,2 | P_emaildomain | R_emaildomain | C1~14 | D1~15 | M1~9 | V1~339
```

---

## 🔗 EDA 
<img width="598" height="488" alt="image" src="https://github.com/user-attachments/assets/8e27b7dc-b25a-46cc-930f-6c64d2ee566c" />

```
class 분포가 굉장히 불균형한 데이터셋
label이 1인 데이터가 전체의 3.5%
```
---
<img width="1990" height="1489" alt="image" src="https://github.com/user-attachments/assets/83d3308e-ca83-4db5-ba00-ea3cc3b3a76c" />

```
id 관련 변수들에 대해 isFraud 타겟변수와의 boxplot
```

---

<img width="584" height="436" alt="image" src="https://github.com/user-attachments/assets/fec0134b-d7a7-490b-81f5-3e5b6fa94e0a" />

```
Transaction Account 값이 공란인지에 따라 fraud 와의 연관성 분석
```
---
<img width="571" height="436" alt="image" src="https://github.com/user-attachments/assets/90eae60a-0505-4e0e-a545-a9b502b4cee5" />

```
ProductCD 가 C인 제품의 사기 비율이 높음
▶️ ProductCD 컬럼을 더미변수화 해서 사용 예정
```
---
<img width="943" height="659" alt="image" src="https://github.com/user-attachments/assets/142a7266-a45d-4f4a-95bc-ed508cb9b64b" />

```
사용하는 이메일 도메인과 사기 여부 분석
사용하는 이메일이 도메인이 흔치 않고 임의의 도메인일 경우, 사기 확률이 높을 것이라는 가설
```
