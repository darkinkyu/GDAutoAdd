# GDAutoAdd

GDAutoAdd is a script which allows users to add to the Google group (or Shared Drive) you specified. It's intended to be deployed to CloudFlare Workers.

## Installation

1. Create a CloudFlare worker and paste the main.js file.
2. Get your client_id, client_secret and refresh_token, paste into `authConfig`.
3. Enable captcha by changing `captcha_config` and add site_key, secret_key into corresponding settings.
4. Enter your Group ID or Shared Drive ID to gd_config. If you want to add users to your group, enter "group" in `gd_config.type`, or enter "drive"
5. Modify `member_filter` section. You can setup AllowList and BlockList to filter users. **member_filter and domain_filter are both working**

## Usage

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
This program is released under license [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)

＃GDAutoAdd

使用GDAutoAdd自助添加用户至您指定的Google组（或Shared Drive）中。该程序应部署至CloudFlare Workers。

##安装

1.创建新的CloudFlare Worker， 并将main.js粘贴进去。
2.获取您的client_id，client_secret和refresh_token，粘贴到authConfig中。
3.通过更改`captcha_config`启用验证码，并将site_key和secret_key添加到相应的设置中。
4.在gd_config中输入您的组ID或共享驱动器ID。 如果要将用户添加到组中，请在`gd_config.type`中输入"group"，或输入"drive"
5.修改`member_filter`部分。 使用白名单和黑名单筛选用户（如需设置单用户名单， 写在"member_filter"里。 域名名单使用"domain_filter"）

##用法

##贡献
欢迎提出请求。 对于重大更改，请先打开一个问题以讨论您要更改的内容。

＃＃ 执照
该程序根据[GPLv3]许可发布（https://www.gnu.org/licenses/gpl-3.0.en.html）
