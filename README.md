# Exegear DB設計


## usersテーブル
|Column|Type|Options|
|------|----|-------|
|nickname|string|null: false|
|email|string|null: false|
|password|string|null:false|
### Association
- has_many :exercises


## exercisesテーブル
|Column|Type|Options|
|------|----|-------|
|workout|string|null: false|
|weight|integer||
|rep|integer||
|memo|text||
|user|references|null: false, foreign_key: true|
### Association
- belongs_to :user


<!-- ※workout:種目 -->
<!-- ※weight:重さ kg -->
<!-- ※rep:回数 -->
<!-- ※memo:メモ -->
