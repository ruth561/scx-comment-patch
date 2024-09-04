# パッチの適用方法

sched_extの開発リポジトリは[ここ](https://git.kernel.org/pub/scm/linux/kernel/git/tj/sched_ext.git/)から入手できる。このパッチは[sched_ext-for-6.11](https://git.kernel.org/pub/scm/linux/kernel/git/tj/sched_ext.git/tag/?h=sched_ext-for-6.11)というタグをベースにしているため、パッチを適用するときはいったんそのタグに移動してから適用するとよい。

※ GitHubに公開されている[sched_extリポジトリ](https://github.com/sched-ext/sched_ext)はややバージョンが低いため注意

```
$ git clone https://git.kernel.org/pub/scm/linux/kernel/git/tj/sched_ext.git
$ cd sched_ext
$ git checkout sched_ext-for-6.11
$ patch -p1 < /path/to/this/repo/add-comments.patch
```
