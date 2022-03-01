## How to run the Flutter Web on GitHub Codespaces.

In this article, I show you how to set up your GitHub codespaces for running the flutter app.

## GitHub Codespaces

GitHub Codespaces is the cloud based development environment provided by GitHub.

https://github.com/features/codespaces

GitHub Codespaces is for now, **For Free** for every individual developers.
(For enterprise or organization, some budgets are required but it's not expensive. See the official website to check the price.)


## Flutter Web

Flutter is officially announced that the Flutter running on the browser becomes **Stable** release from ver.2.5. (And, now Flutter has already release 2.10.0 as stable. Awesome development speed!! )

Flutter Web is the good option to check and learn your flutter code even if you don't use web production.


## Flutter Web on GitHub Codespaces


First, create new repository on your GitHub.  And run "New codespaces" on your repository.

![flutter-web-sandbox-github-repository](https://cdn.hashnode.com/res/hashnode/image/upload/v1646146087344/kNbxdZ3II.png)


After 20-30 seconds, you can get the following online editor view like VSCode.

![github-codespaces-demo](https://cdn.hashnode.com/res/hashnode/image/upload/v1646146176747/n1vvDJiyx.png)


Next, to install the flutter SDK. I recommend you to install FVM (Flutter Version Manager tool).

https://fvm.app/

To install the FVM, you need to install the Homebrew. This setup ways are explains on the above FVM official website, so I skip the explanation here.

After installing FVM, you can install any version's SDK via **fvm** commands. 

```shell
$> fvm flutter install stable
```

Next, create new flutter app.

```shell
$> fvm flutter create my_app
```

Then, run the flutter web app on the browser.

```shell
$> fvm flutter run -d web-server --web-hostname=0.0.0.0 --web-port=3000
```

That's all.

Let's enjoy Flutter Web on GitHub codespaces, from any devices!!






