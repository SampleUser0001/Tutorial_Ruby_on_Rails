# Tutorial Ruby on Rails

## 新しいページを作成する

1. ```config/routes.rb```に記載
    ``` rb
    Rails.application.routes.draw do
      get "/articles", to: "articles#index"
    
      # For details on the DSL available within this file, see https://guides.rubyonrails.org/routing.html
    end
    ```
2. 下記実行
    ``` bash
    rails generate controller Articles index --skip-routes
    ```
3. ```app/views/articles/index.html.erb```作成

## 参考

- [Getting Started with Rails -- Rails Guild](https://guides.rubyonrails.org/getting_started.html)