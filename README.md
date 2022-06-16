# Interval 🤝 Render

An example project with [Interval](https://interval.com) configured to run on [Render](https://render.com). Created with [create-interval-app](https://github.com/interval/create-interval-app).

Click the button below to deploy this app to your Render account:

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/interval/interval-render)

In this configuration we're deploying to a single [Background Worker](https://render.com/docs/background-workers). This is also how we power our own internal tools here at Interval! Running our tools as a separate service with auto-deploys enabled means we can update our tools much more frequently than we push updates to the production app.

Important settings: (also defined in [render.yaml](https://github.com/interval/interval-render/blob/main/render.yaml))

- **Service type:** worker
- **Environment:** node
- **\# of instances:** 1
- **Build command:** `yarn && yarn build`
- **Start command:** `yarn start`

### Helpful links

- [Interval](https://interval.com)
- [Render](https://render.com)
- [Interval documentation](https://interval.com/docs)

### Typing

The Interval SDK is written in TypeScript and should have rich type hints and inference. If you experience issues with IDE support, please ensure your editor is using the correct version of TypeScript that is installed in the workspace. If you are using Visual Studio Code, please try [using the workspace version of TypeScript](https://code.visualstudio.com/docs/typescript/typescript-compiling#_using-the-workspace-version-of-typescript). Many editors should do this automatically.

If that doesn't help, please let us know! hello@interval.com
