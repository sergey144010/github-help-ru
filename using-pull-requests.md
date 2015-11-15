Адрес статьи:
https://help.github.com/articles/using-pull-requests/

# Использование Pull Requests

Пулл запросов позволяет Вам рассказать другим о Ваших изменениях отправленных в репозиторий на GitHub.
Когда pull request был отправлен, заинтересованные стороны могут проанализировать совокупность изменений, обсудить возможные изменения, и зафиксировать их при необходимости (событием push).

Это руководство проведет через процесс отправки гипотетического патча с использованием различных ревью кода и инструментов управления, чтобы зафиксировать изменения.

++++++++++++++++++++++++++++++++++++
<font style="background-color:red">
Pull requests let you tell others about changes you've pushed to a repository on GitHub. Once a pull request is sent, interested parties can review the set of changes, discuss potential modifications, and even push follow-up commits if necessary.

This guide walks through the process of sending a hypothetical pull request and using the various code review and management tools to take the change to completion.
</font>

++++++++++++++++++++++++++++++++++++

## Прежде чем начать

Это руководство предполагает, что у Вас есть аккаунт на GitHub, что Вы сделали ответвление (fork) от некоего существующего репозитория, и что Вы сделали изменения в Вашем ответвлении и они помещены на GitHub (push). Справка по ответвлениям и сохранениям изменений в разделе Forking a Repo.

++++++++++++++++++++++++++++++++++++

Before you begin

This guide assumes that you have a GitHub account, that you've forked an existing repository, and that you've pushed changes to your fork. For help with forking and pushing changes, see the Forking a Repo article.

++++++++++++++++++++++++++++++++++++

## Инициирование pull request

В следующем примере Hubot завершил некоторые работы с ответвлением Octocat's Spoon-Knife репозитория, отправил изменения на GitHub (операциии - commit и push) в своё ответвление (в свою вилку, в свой fork) и хочет комуто показать сделанные изменения и объединить свои изменения (в своём fork) с исходным репозиторием.

Перейдите в свой репозиторий с изменениями которые Вы хотите отправить и нажмите кнопку Pull Request.

1. Переключите Вашу ветку.
2. Нажмите кнопку Compare & review.

Pull Request могут быть посланы из любой ветки или фиксации (commit), но рекомендуется использовать тематическую ветку, чтобы последующие фиксации (commit) можно было сдвигать при необходимости.

++++++++++++++++++++++++++++++++++++

Initiating the pull request

In the following example, Hubot has completed some work on a fork of the Octocat's Spoon-Knife repository, pushed a commit to a topic branch in his fork, and would like someone to review and merge.

Navigate to your repository with the changes you want someone else to pull and press the Pull Request button.

    Branch selection dropdownSwitch to your branch
    Pull Request buttonClick the Compare & review button

Pull requests can be sent from any branch or commit but it's recommended that a topic branch be used so that follow-up commits can be pushed to update the pull request if necessary.

++++++++++++++++++++++++++++++++++++

## Обзор pull request

После запуска обзора, Вы увидите комментарии на странице, там же можно получить высокоуровневый обзор того, что именно изменилось между Вашей веткой и веткой репозитория Master.
Вы можете просмотреть все комментарии, сделанные на коммиты (фиксации - commit), определить, какие файлы изменены, и получить список участников в Вашей ветке.

++++++++++++++++++++++++++++++++++++

Reviewing the pull request

After starting the review, you're presented with a review page where you can get a high-level overview of what exactly has changed between your branch and the repository's master branch. You can review all comments made on commits, identify which files changed, and get a list of contributors to your branch.

++++++++++++++++++++++++++++++++++++

Changing the branch range and destination repository

By default, pull requests are assumed to be based on the parent repository's default branch. In this case, the hubot/Spoon-Knife repository was forked from octocat/Spoon-Knife so the pull request is assumed to be based on the master branch of the octocat/Spoon-Knife repository.

In many cases, the defaults are appropriate. If necessary, you can change the parent repository and branch with the drop-down lists. Clicking on Edit at the top allows you to swap between your head and base, as well as establishing diffs between various reference points. References here must be branch names in your GitHub repository.

The easiest way of thinking about the branch range is this: the base branch is where you think changes should be applied, the head branch is what you would like to be applied.

Changing the base repository changes who is notified of the pull request. Everyone that can push to the base repository will receive an email notification and see the new pull request in their dashboard the next time they sign in.

When you change any of the info in the branch range, the commit and files changed preview areas will update to show your new range.

Using the compare view, you can set up comparisons across any arbitrary timeframe.

++++++++++++++++++++++++++++++++++++