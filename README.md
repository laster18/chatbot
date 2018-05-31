# DB設計

## dictionariesテーブル

|Column|Type|Options|
|------|----|-------|
|request|text|null: false|
|response|text|null: false|


## historiesテーブル

|Column|Type|Options|
|------|----|-------|
|user_input|text|null: false|
|bot_response|text|null: false|
|response_timestamp|date|null: false|


# ルーティング

- GET root => 'chats#index'
- POST /chat => 'chats#create'
- GET /history => 'histories#index'

# コントローラー

- chats
- histories

# models

- History
- Dictionary
