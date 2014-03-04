关于hexo deploy失败的问题，大部分是因为/data/software/node-v0.11.11/lib/node_modules/hexo/lib/plugins/deployer/github.js里的一行代码写得太死的原因：

```
function(next){
      var commands = [
        ['add', '-A'],
        ['commit', '-m', new Date().getTime()],
        ['push', 'origin', config.branch, '--force']
      ];

      async.forEachSeries(commands, function(item, next){
        console.log('执行git ', item.join(' '));
        command('git', item, next);
      }, next);
}
```

自己的repository迁移下来时用的`git remote add origin 我的项目仓库`，而源码中的` ['push', 'github', config.branch, '--force']`用的是github，于是就push不到github了。
