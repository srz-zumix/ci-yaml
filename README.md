# ci-yaml

## ci service yaml

|CI|Status|YAML config|Alias|Merge|Lint|KB|
|:--|:--|:--|:--|:--|:--|:--|
|[AppVeyor](https://www.appveyor.com)|[![Build status](https://ci.appveyor.com/api/projects/status/heqex7sf0bvi7pox?svg=true)](https://ci.appveyor.com/project/srz-zumix/ci-yaml)|[YES](https://www.appveyor.com/docs/appveyor-yml/)|YES|NO|[Validate YAML configuration](https://ci.appveyor.com/tools/validate-yaml)||
|[Azure Pipelines](https://azure.microsoft.com/ja-jp/services/devops/pipelines/)|[![Build Status](https://dev.azure.com/srz-zumix/ci-specs/_apis/build/status/ci-yaml-CI?branchName=master)](https://dev.azure.com/srz-zumix/ci-specs/_build/latest?definitionId=8&branchName=master)|[YES](https://docs.microsoft.com/en-us/azure/devops/pipelines/yaml-schema?view=azure-devops&tabs=schema)|NO|NO|[YAML Schema](https://docs.microsoft.com/en-us/azure/devops/pipelines/yaml-schema?view=azure-devops&tabs=schema)|[KB](https://github.com/srz-zumix/ci-yaml/labels/Azure%20Pipelines)|
|[Bitrise](https://www.bitrise.io)|[![Build Status](https://app.bitrise.io/app/bccdcec7b8beb3cf/status.svg?token=3mtflyXOuH8Ahx3q-OJbNA)](https://app.bitrise.io/app/bccdcec7b8beb3cf)|[Can](https://devcenter.bitrise.io/tips-and-tricks/use-bitrise-yml-from-repository/)|||
|[Buddy](https://buddy.works)|[![buddy branch](https://app.buddy.works/zumixcpp/ci-yaml/repository/branch/master/badge.svg?token=5e58135ab4831252209e7b1fe75bfe9de669b0dc7e95ed4316eebad2187d59a0 "buddy branch")](https://app.buddy.works/zumixcpp/ci-yaml/repository/branch/master)|YES|NO|NO|[YAML Schema](https://buddy.works/knowledge/yaml/yaml-schema)|[KB](https://github.com/srz-zumix/ci-yaml/labels/Buddy.works)|
|[Circle CI](https://circleci.com)|[![CircleCI](https://circleci.com/gh/srz-zumix/ci-yaml.svg?style=svg)](https://circleci.com/gh/srz-zumix/ci-yaml)|YES|YES|YES|[circleci config validate](https://circleci.com/docs/2.0/local-cli/#validate-a-circleci-config)||
|[Cirrus CI](https://cirrus-ci.org/)|[![Build Status](https://api.cirrus-ci.com/github/srz-zumix/ci-yaml.svg)](https://cirrus-ci.com/github/srz-zumix/ci-yaml)|YES|YES|YES|-||
|[Codefresh](https://codefresh.io/)|[![Codefresh build status](https://g.codefresh.io/api/badges/pipeline/srz-zumix/srz-zumix%2Fci-yaml%2Fci-yaml?branch=master&key=eyJhbGciOiJIUzI1NiJ9.NThhNTFmYzlkZjcwMWYwMTAwNjNlYjY3.U-q8LiP3IK9DLygcIx5UOa015KH690k8u3uiLINI9tw&type=cf-1)](https://g.codefresh.io/pipelines/ci-yaml/builds?repoOwner=srz-zumix&repoName=ci-yaml&serviceName=srz-zumix%2Fci-yaml&filter=trigger:build~Build;branch:master;pipeline:5c82394690bbd7dccfae2529~ci-yaml)|YES|YES|YES|[Yaml validation](https://codefresh.io/docs/docs/codefresh-yaml/what-is-the-codefresh-yaml/#yaml-validation)||
|[Codeship](https://codeship.com/)|[![Codeship Status for srz-zumix/ci-yaml](https://app.codeship.com/projects/4dd06940-2384-0137-7251-26e7151593a1/status?branch=master)](https://app.codeship.com/projects/329959)|Pro only|||
|[Drone Cloud](https://cloud.drone.io/)|[![Build Status](https://cloud.drone.io/api/badges/srz-zumix/ci-yaml/status.svg)](https://cloud.drone.io/srz-zumix/ci-yaml)|YES|YES|YES|[drone-yaml lint](github.com/drone/drone-yaml)|[KB](https://github.com/srz-zumix/ci-yaml/issues?q=is%3Aissue+is%3Aopen+label%3ADrone)|
|[Rocro](https://rocro.com/)|[![Job Status](https://inspecode.rocro.com/badges/github.com/srz-zumix/ci-yaml/status?token=LuMtO5aKfnnbmhXx60alSosyMAJg8xHlOAlU5blg8DE)](https://inspecode.rocro.com/jobs/github.com/srz-zumix/ci-yaml/latest?completed=true)|YES|YES|YES|-||
|[Scrutinizer](https://scrutinizer-ci.com)|[![Build Status](https://scrutinizer-ci.com/g/srz-zumix/ci-yaml/badges/build.png?b=master)](https://scrutinizer-ci.com/g/srz-zumix/ci-yaml/build-status/master)|YES||
|[Semaphore CI](https://semaphoreci.com)||NO|||
|[Semaphore CI 2.0](https://semaphoreci.com/product)||[YES](https://docs.semaphoreci.com/article/50-pipeline-yaml)|YES|NO||
|[Shippable](http://shippable.com)|[![Run Status](https://api.shippable.com/projects/5c81c714b2f57f060005ea49/badge?branch=master)]()|YES|YES|YES|[FAQ](http://docs.shippable.com/getting-started/support/#how-can-i-validate-my-shippable-yml)||
|[Travis CI](https://travis-ci.com/)|[![Build Status](https://travis-ci.com/srz-zumix/ci-yaml.svg?branch=master)](https://travis-ci.com/srz-zumix/ci-yaml)|YES|YES|NO|[travis lint](https://github.com/travis-ci/travis.rb#lint)|[KB](https://github.com/srz-zumix/ci-yaml/labels/Travis%20CI)|
|[wercker](http://www.wercker.com/)|[![wercker status](https://app.wercker.com/status/d3bc651ac712a5efaac4ff709ae244c6/s/master "wercker status")](https://app.wercker.com/project/byKey/d3bc651ac712a5efaac4ff709ae244c6)|Partial(Pipeline)|YES|YES|[YAML Syntax](http://devcenter-staging.wercker.com/docs/wercker-yml/yaml-syntax.html)||

## YAML Anchor/Alias

### Anchor/Alias 

```yaml
hoge: &test #anchor
fuga: *test #alias
```

### Merge

```yaml
hoge: &test #anchor
  name: hoge
  env:
    HOGE: 1
  command:
    - echo $HOGE
fuga:
  <<: *test #merge
  env:
    HOGE: 0
```

### Array Anchor/Alias

```yaml
- &test #anchor
  name: hoge
  command: echo hello
- *test #alias
```
