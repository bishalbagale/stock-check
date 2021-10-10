# stock-check
`stock-check`  is simple shell script that notifies user about the stock price when it exceeds certain threshold. 

---
### Install
Please install and configure [`telegram-send`](https://github.com/rahiel/telegram-send) in your system.

---
### usage
```
❯ ./stock-check --help                                                    
 Syntax: stock-check [-c|t|T|h]

 options:
	-c	        company symbol [required!]
 	-t	        time(sec).. check stock vlaue in every t(sec) [optional / default 300s ]
	-T              threshold value of stock price for the notification to be sent [optional / default 0]
 	-h | --help	to view this help menu

 example1: stock-check -c XYZ -t 300
 		notifies stock value of XYZ every 300s i.e.5 min

 example2: stock-check -c XYZ -t 300 -T 2000
		checks the stock value every 300s but notifies only when the vlaue exceeds or equals 2000

NOTE: PLEASE MAKE SURE YOU HAVE telegram-send INSTALLED AND CONFIGURED IN YOUR SYSTEM.

```
