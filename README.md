# OS_Forg (修課時間為2014年...)
## OS修課的第二次作業

### 青蛙過河是一款大家耳熟能詳的小遊戲...
### 內容是: 你要控制一隻不知道為什麼不會游泳的青蛙,不斷地跳過河上的漂流木,漂到對岸去,則算成功
### 解說 :   圖示如下 以*代替青蛙, ====  是陸地    ---是漂流木 每一根漂流木的長度會隨機產生  另外,每次開始遊戲時,每個河道的漂流木的方向會被隨機決定
### 每一秒木頭會移動(透過螢幕的刷新),每個河道的漂流木速度隨機設定 (可能一秒一次移動三格?)
          
# ===============================
#   - - - --    -- - - -- - - - -- - - - --    -- - - -- - - - -- - - - --    -- -
#      -- --    -- -- --      -- -- -- -- --    -- -- --      -- -- -- -- --    -- -
#         ----    -- -- --    -- -- --  - ----    -- -- --    -- -- -----    -- -- -- 
#         ----    ------    -- -- ---------    ------    -- -    ------    -- -- ------   
#         -- --    -- -- --    -- -- ---- --    -- -- --    -- -- ---- --    -- -- --    -- 
# ==============*===============.
    
         
                
### 實作想法 :  因作業要求使用Pthread   
### 因此在規劃後使用三個pThread,分別控制青蛙的移動,漂流木的移動,以及監聽使用者敲擊鍵盤動作.
### 一開始在處理同步的部分沒處理好,所以我的青蛙是斜著跳的~~哈哈~~

