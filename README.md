# Check 996

Help your check repo 996 status. 😎

```
Usage: count_code.rb [options]
    -s, --start WORK_START_TIME      start job time e.g. 10:00:00
    -e, --end WORK_END_TIME          end job time  e.g. 18:00:00
    -g, --git-log GIT_LOG_CMD        use git log command, default is `git log --all`
    -f, --filter FILTER              time range filter  e.g. last_[day|week|month|year] last_5_[day|week|month|year]   '2022-01-01 08:10:00,2022-10-01 08:10:00'
    -v, --version                    version
```

# Use

## System dependency

make sure you have  `ruby 2.7+`, `curl` or `wget` will be helpful.
### step1:

cd your git code repo directory.

```bash
cd </path/to/your/git_repo>
```

### step2: 

run this code.

* curl support

```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Mark24Code/check_996/main/check_996.rb)"
```

* wget support

```bash
ruby -e "$(wget https://raw.githubusercontent.com/Mark24Code/check_996/main/check_996.rb -O -)"
```

## Tips：

remote run add params 

```
 <script>  -- -s 10:30 -e 19:30
```

e.g.

```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Mark24Code/check_996/main/check_996.rb)" -- -s 10:30 -e 19:30
```
