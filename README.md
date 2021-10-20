# README
DB設計
#  calendarsテーブル
| Column              | Type       | Options                   |
| ------------------- | ---------- | --------------------------|
| name                | string     | null: false               |
| color               | string     |                           |
| visibility          | boolean    |                           |

### Association
- has_many : events

## events テーブル
| Column          | Type       | Options                        |
| --------------- | ---------- | ------------------------------ |
| name            | string     | null: false                    |
| color           | string     |                                |
| description     | text       |                                |
| start           | datetime   | null: false                    |
| end             | datetime   | null: false                    |
| timed           | boolean    |                                |

### Association
- belongs_to : calendar