# README

## usersテーブル

|Column|Type|Options|
|------|----|-------|
|name|string|null: false, foreign_key: true|
|email|string|null: false, foreign_key: true|
|password|string|null: false, foreign_key: true|

### Association
- belongs_to :messages
- belongs_to :groups

## messagesテーブル

|Column|Type|Options|
|------|----|-------|
|text|t.text|null: false, foreign_key: true|
|users|string|null: false, foreign_key: true|
|groups|string|null: false, foreign_key: true|
|image|string|null: false, foreign_key: true|

### Association
- belongs_to :users
- belongs_to :groups

## groupsテーブル

|Column|Type|Options|
|------|----|-------|
|text|t.text|null: false, foreign_key: true|
|users|string|null: false, foreign_key: true|
|name|string|null: false, foreign_key: true|

### Association
- belongs_to :users
- belongs_to :messages



