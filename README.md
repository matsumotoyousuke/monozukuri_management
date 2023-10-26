## usersテーブル
|Column             |Type   |Options                   |
|-------------------|-------|--------------------------|
|name               |string |null: false               |
|email              |string |null: false, unique: true |
|encrypted_password |string |null: false               |

### Association
- has_many :comments
- has_many :informations

## commentsテーブル
|Column             |Type   |Options                   |
|-------------------|-------|--------------------------|
|
|
|