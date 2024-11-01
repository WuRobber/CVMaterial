# 虛擬實境遊戲設計專案
這個 Unity 專案的目標是打造一個擬真的台大校園 VR 環境，融合互動和動畫效果，提升沉浸式體驗。以下是專案的主要元素及互動設計：

1. 場景 (Scene)
本專案將以台大校園為場景，重現校園的典型風貌。環境中包含各式校園設施、自然景觀及隨機出現的校園角色，讓用戶仿若置身其中。

2. 動畫效果 (Animations)
太陽旋轉動畫：當太陽處於待機狀態時，會緩慢旋轉，模擬日照的自然運行。
路人待機動作：校園中的路人角色會各自做出不同的待機動作，如低頭滑手機、聊天等，讓場景更為生動。
貓咪待機動畫：在校園內可以看到待機狀態的貓咪，模擬真實環境中的動物互動。
角色待機及移動動畫：主角在待機時會顯示 idle 動畫，當用戶按下鍵盤上的 WASD 鍵時，角色會根據方向顯示相應的移動動畫。
3. 觸發器 (Triggers)
弓箭觸碰太陽消失：用戶可以用滑鼠發射弓箭，當弓箭與太陽相碰時，太陽會消失，增添互動樂趣。
WASD 鍵盤觸發角色移動：按下鍵盤上的 W、A、S、D 鍵時，角色會移動並播放對應的行走動畫。
滑鼠按鍵觸發弓箭發射：用戶點擊滑鼠按鍵即可發射弓箭，體驗角色的攻擊操作。
4. 其他設定 (Other Settings)
弓箭飛行距離與停留時間：在設置界面中，可以設定弓箭的最大飛行距離及停留時間，使弓箭具有真實的物理效果和互動性。
OnCollision 事件：在弓箭與太陽間建立 OnCollision 事件，確保兩者接觸時會觸發消失動畫，使互動順暢且更具趣味性。

本專案結合動畫效果、互動觸發及場景還原，旨在提供用戶沉浸式體驗，讓他們在 VR 中感受到校園生活的活力與趣味。

---

# Demo Video

- [Watch on YouTube](https://youtu.be/u8HGTndaenk)

---

# Download Unity Project

- [Download from Google Drive](https://drive.google.com/file/d/1PD8vAn82RE4mANSXcwBHljaD0aH4awA4/view?usp=sharing)

