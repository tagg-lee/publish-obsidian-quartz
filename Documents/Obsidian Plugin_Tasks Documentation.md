---
aliases: 
created: 2023-10-19
tags:
  - Obsidian-app
---

# 옵시디언 플러그인 - Tasks Documentation
- [[Obsidian Plugin_Tasks_Recursive task|반복되는 Task 만들기]]

## Queries Examples

#### `Effort` 폴더에 완료되지 않은 Task 불러오기
> ```tasks
> not done
> folder includes Effort
> ```

#### 오늘 완료한 Task 불러오기
>[!Done] What i've done today
>```tasks
filter by function task.done.format("YYYY-MM-DD") == moment().format("YYYY-MM-DD")
hide done date
>sort by done
>```