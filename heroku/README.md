# Graph API Webhooks Heroku Sample

This is a sample client for Facebook's [Webhooks](https://developers.facebook.com/docs/graph-api/webhooks/) product and Instagram's [Subscriptions API](https://www.instagram.com/developer/subscriptions/), powered by [Node.js on Heroku](https://devcenter.heroku.com/articles/getting-started-with-nodejs).

## Setup

### Facebook Webhooks

1. Refer to Facebook's [Webhooks sample app documentation](https://developers.facebook.com/docs/graph-api/webhooks/sample-apps) to see how to use this app.
1. Deploy the sample app on Heroku with this button:

    [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/fbsamples/graph-api-webhooks-samples)

### Instagram Subscription API
1. Register an [Instagram API client](https://instagram.com/developer/clients/manage/).
1. Deploy the sample app on Heroku with this button:

    [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/fbsamples/graph-api-webhooks-samples)

1. Set up your client's [subscription](https://www.instagram.com/developer/subscriptions/) using your `https://<your-subdomain>.herokuapp.com/instagram` as the callback URL. It is recommended that you set a `TOKEN` [config var](https://devcenter.heroku.com/articles/config-vars) as part of the set up of your Heroku app to secure requests. If you choose not to set a config var, then you will need to set a verify token of 'token' when configuring the callback URL.

### Memo

- env settings  
    - process.env.PORT: ポート
    - process.env.APP_SECRET: Facebookのアプリの[アプリダッシュボード](https://developers.facebook.com/apps)から取得
    - process.env.TOKEN: 任意の文字列。未設定の場合は"token"。
    - process.env.SLACK: slackのwebhook。発行方法はこちらを[参照](https://docs.trocco.io/s/article/Slack%E3%81%A7Webhook-URL%E3%82%92%E7%99%BA%E8%A1%8C%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95?language=ja)

- [Webhooks](https://developers.facebook.com/docs/graph-api/webhooks)

- [Slack通知をNode.jsでもやってみる](https://ccbaxy.xyz/blog/2020/01/14/node2/) 


