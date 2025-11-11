# UAV and mmWave Operation in CF mMIMO

---

## UAVs in Future Wireless Networks

- UAVs (Unmanned Aerial Vehicles) act as **flying base stations**.  
- Can dynamically move to **fill coverage holes** and enhance capacity.  
- Offer **Line-of-Sight (LoS)** advantage compared with ground APs.  
- Increasingly used in **surveillance, delivery, and communications**.

####

- UAV（無人航空機）は**飛行型基地局**として機能。  
- **通信エリアの空白**を補い、ネットワーク容量を向上させる。  
- 地上APに比べて**見通し通信（LoS）**が得やすい。  
- **監視・配送・通信**など多様な分野で利用が拡大中。

---

## UAVs as Users in CF mMIMO ([136][137])

- CF mMIMO = many distributed APs jointly serve all users (no cells).  
- Enables **stable uplink/downlink** even for high-altitude UAVs.  
- [136][137] show: **CF mMIMO outperforms conventional systems**.  
- Especially **robust at high altitudes** due to no cell-edge interference.

####

- CF mMIMO = 多数の分散APがセル境界なしで全ユーザを協調サポート。  
- 高高度UAVでも**安定した上り・下りリンク**を実現。  
- 文献[136][137]は、**従来方式より優れた性能**を示している。  
- セル境界干渉がないため、**高高度で特に安定性が高い**。

### Fig.6 — UAV UL Rates under Different Architectures ([136])

CF mMIMO achieves higher UL rates for UAVs than traditional cellular mMIMO and user-centric mMIMO,  
as shown by the right-shifted blue curves in the CDF.  
This demonstrates its superior interference management and consistent link quality.  

####

CF mMIMO は cellular mMIMO および user-centric mMIMO よりも UAV の上りリンク速度が高く、  
CDF の青い曲線の右方向シフトにより、干渉抑制とリンク安定性の優位性を示している。  

![136_Fig6](../images/136_fig6.png)


---

## UAV-Aided CF mMIMO ([138][139])

- UAVs can **assist networks** (not only act as users).  
- [138]: UAV + Aerial RIS (AIRS) improves DL rate for users in bad channels.  
- Jointly optimize **UAV position + RIS reflection phase**.  
- [139]: UAV as **mobile base station (MBS)** for CF mMIMO cooperation.  
- Uses **trajectory optimization + power control** to enhance QoS.

####

- UAVは**ユーザとしてだけでなく、ネットワーク支援装置**にもなる。  
- [138]: UAVに**空中RIS（AIRS）**を搭載 → 悪条件ユーザのDLレートを改善。  
- **位置＋反射位相の同時最適化**で性能を向上。  
- [139]: UAVを**移動型基地局**として利用し、CF mMIMOと連携。  
- **軌道最適化＋電力制御**で全体のQoSを改善。

### Fig.7 — Performance Comparison with/without AIRS ([138])
 
With AIRS location optimization, the achievable DL rate increases dramatically.  
Joint optimization of UAV position, AP beamforming, and AIRS phase shift leads to higher efficiency.  

#### 
AIRS 位置を最適化することで DL レートが大幅に向上。  
UAV の位置、AP ビームフォーミング、および AIRS 位相の同時最適化による効果を示す。  

![138_Fig7](../images/138_fig7.png)
 

### Fig. 6 — System Throughput vs. Number of APs ([139])

MBS-assisted CF mMIMO shows significant throughput gain over conventional CF mMIMO by joint trajectory and power optimization.
####
軌道 および 電力 の最適化により、MBS支援 CF mMIMO が従来方式より高い スループット を達成。

![139_Fig6](../images/139_fig6.png)

---

## Comparison and Summary

**UAV as User ([136][137])**  
→ CF mMIMO enhances UAV DL/UL rates via cooperative APs.  
**UAV as Helper ([138][139])**  
→ UAVs with RIS or MBS functions improve system QoS.  

####

**UAVをユーザとして扱う場合 ([136][137])**：  
→ CF mMIMOの協調によりUAVの上下リンク性能が向上。  
**UAVを支援側として扱う場合 ([138][139])**：  
→ RIS搭載や移動基地局化によりシステム全体のQoSを改善。  

###

Together these studies show UAVs can both **benefit from** and **enhance** CF mMIMO systems.  

これらの研究は、UAVがCF mMIMOの恩恵を受けるだけでなく、ネットワークを強化する側にもなり得ることを示しています。  

| Role of UAV | References | Key Focus | Main Finding |
|--------------|-------------|------------|---------------|
| As User | [136], [137] | Compare CF vs. Cellular MIMO | CF improves UAV DL/UL rates |
| As Helper / BS | [138], [139] | Optimize UAV position, RIS, and power | Improves overall system QoS |

---

## CF mMIMO in mmWave Bands — Overview ([140])

- High-frequency bands such as **mmWave, terahertz, optical wireless** are key technologies for **5G and beyond**.  
- Offer **immense bandwidth** compared with sub-6 GHz microwave bands.  
- **CF mMIMO** in these bands leverages **short wavelengths** to pack many antennas in small areas.  
- This allows **fine-grained narrow beams**, significantly improving communication links [140].
####
- **ミリ波・テラヘルツ・光無線**などの高周波数帯は、**5G以降の通信**を支える重要技術。  
- **サブ6 GHz帯より広い帯域幅**を提供。  
- **短波長**を活かして、**高密度アンテナ配列**が可能。  
- **精密な狭ビーム形成**により通信品質が大幅に向上 [140]。

### Fig. 38 — Number of Antenna Elements vs Frequency ([140])
Higher frequencies require more antennas to compensate for greater path loss.  
####
周波数が高くなるほどパスロス補償のために必要なアンテナ数が増加。  

![140_Fig38](../images/140_fig38.png)


---

## Candidate mmWave Frequency Bands for 5G and Beyond ([141])

- The **mmWave spectrum (3 – 300 GHz)** includes both *super high* (3–30 GHz) and *extremely high* (30–300 GHz) bands.  
- The **FCC (2016)** designated specific bands for 5G mobile broadband [141]:  
  - **28 GHz band (27.5 – 29.5 GHz)** → ~1 GHz available for mobile broadband.  
  - **70 – 80 GHz bands (E-band)** → 10 GHz total for backhaul and mobile links.  
  - **90 GHz band (W-band)** → 92 – 100 GHz for fixed and mobile services.  
- **Total available bandwidth: 24 GHz** for future high-capacity wireless systems.

####
- **ミリ波帯 (3〜300 GHz)** には、超高周波 (3〜30 GHz) と極超高周波 (30〜300 GHz) が含まれる。  
- **FCC (2016)** は 5G 移動通信向けに次の帯域を割り当て [141]：  
  - **28 GHz 帯 (27.5〜29.5 GHz)** → 約 1 GHz が モバイル通信 向け。  
  - **70〜80 GHz 帯 (E バンド)** → 合計 10 GHz が バックホール 通信 と 移動 通信 に 利用。  
  - **90 GHz 帯 (W バンド)** → 92〜100 GHz が 固定 ・ 移動 通信 に 利用。  
- **総利用可能帯域幅 24 GHz** → 将来の大容量通信に有望。

