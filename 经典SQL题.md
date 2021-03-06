### 1. 给定一张日志表，有3个字段 user_id / page_id / access_time，给出用户的访问路径。
输入: aaabbaac，输出：abac  

### 2. 给定一张日志表，有4个字段 user_id / session_id / page_id / access_time，需要计算用户在每个页面的停留时长

### 3. 给定一张用户关注表 T，假设用户 a 关注用户 b，则 from_id 是 a，to_id 是 b，如果 ab 互相关注，则表T里存在两条记录 a b 和 b a，现假设表 T 里均为互相关注的记录，如何只保留互相关注记录中的一条？随机取一条即可
输入：
| from_id | to_id |
| -- | -- |
| a | b |
| b | a |  

输出：
| from_id | to_id |
| -- | -- |
| a | b |

或
| from_id | to_id |
| -- | -- |
| b | a |


