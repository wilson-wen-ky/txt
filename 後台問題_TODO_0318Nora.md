###### tags: `TODO`

# TODO
## ＳＰ文件問題
 1. 查找並表列出無效或遺失的ＳＰ檔案
 2. 查找ＳＰ檔案使用參數的有效性及確認使用的ＤＢ內容
 3. 查找innoDb 轉為federated table時遺漏未補的ＤＢ資料
 4. 描述個別問題對Ｃ端code的影響
### list sp info
| spName | spFromWhichDB | spParam | spFromDao | spFromScreen |
|----|----|----|----|----|
| sp_GetGameRecord2 | KYDB_NEW | 14 | winandLoseReportDao.js | winAndLoseReport.js |
- spParam:
        beginDate: beginDate,
        endDate: endDate,
        kindId: options.req.query.kindId || 0,
        accounts: accounts,
        serverId: options.req.query.serverId || 0,
        ChannelID: options.req.session.user.isagent == 1 ? options.req.session.user.id : 0,
        limit: options.req.query.limit || 0,
        offset: options.req.query.offset || 0,
        total: options.req.query.total || 0,
        isPage: options.isPage,
        isStatis: options.isStatis,
        gameNo: GameUserNO,
        Timezone: Timezone,
        RoomType: RoomType



## 將ＧＣＰ(romeoandjuliet)作為獨立的補強專案，與Lyworkspace分開建立獨立server

## ssh堡壘機只使用 game-lync2-dev-tw 內的lyworkspace進行查詢參考
