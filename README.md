# Notifications service Ansible role [![Ansible Lint](https://github.com/namelivia/ansible-notifications-service/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/namelivia/ansible-notifications-service/actions/workflows/ansible-lint.yml)

## This is a WIP

The project depends on the collection `community.docker` but apparently this [cannot be listed as a dependency](https://github.com/ansible/ansible/issues/62847) so make sure you add it to your `requirements.yml` file like:

```yml
---

collections:
  - community.docker

roles:
  - src: https://github.com/namelivia/ansible-notifications-service
```

## Required variables
 - `cloudwatch_region` Cloudwatch region to send the logs to.
 - `cloudwatch_log_group` Cloudwatch log group to send the logs to.
 - `notifications_telegram_api_id` Your telegram API ID.
 - `notifications_telegram_chat_id` The chat id you are sending your notifications to.
 - 
# IMPORTANT

This project is not maintained anymore and the repository is being archived. The reason why is because this was trying to implement what [Apprise](https://github.com/caronc/apprise) is already doing.
So use [Apprise](https://github.com/caronc/apprise) instead, since it is a more mature project.
