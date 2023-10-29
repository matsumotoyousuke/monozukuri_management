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
|Column      |Type       |Options                        |
|------------|-----------|-------------------------------|
|content     |text       |null: false                    |
|information |references |null: false, foreign_key: true |
|user        |references |null: false, foreign_key: true |

### Association
- belongs_to :user

## informationsテーブル
|Column   |Type       |Options                        |
|---------|-----------|-------------------------------|
|process  |           |null: false
|drawing  |           |
|document |           |
|stock    |           |
|budget   |           |
|minutes  |           |