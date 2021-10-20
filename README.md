# README
DB設計
#  calendarsテーブル
| Column              | Type       | Options                   |
| ------------------- | ---------- | --------------------------|
| name                | string     | null: false               |
| visibility          | boolean    |                           |

### Association
- has_many : events

## events テーブル
| Column          | Type       | Options                        |
| --------------- | ---------- | ------------------------------ |
| name            | string     | null: false                    |
| description     | text       |                                |
| start           | datetime   | null: false                    |
| end             | datetime   | null: false                    |
| timed           | boolean    |                                |

### Association
- belongs_to : calendar