### 获取特定时间
- $ date --date="now"   // 現在時間
- $ date --date="yesterday"  // 昨天
- $ date --date="1 days ago"  // 昨天
- $ date --date="3 days ago"  // 三天前
- $ date --date="tomorrow" // 明天
- $ date --date="1 days" // 明天
- $ date --date="3 days" // 三天後
- 

### 格式
- "_"：0用空白填塞
- "-"：0不填塞
- "^"：输出全部为大写
```
// "^"的区别
date --date="3 days"  +"%Y %_m-%d, %a ,%H:%-M"
2019  4-22, Mon ,20:39
date --date="3 days"  +"%Y %_m-%d, %^a ,%H:%-M"
2019  4-22, MON ,20:39

// "_"的区别
date --date="3 days"  +"%Y %_m-%_d, %H:%_M"
2019  4-22, 20:35
date --date="3 days"  +"%Y %m-%_d, %H:%_M"
2019 04-22, 20:35
```
