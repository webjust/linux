# VIM按键说明 #

## 工作模式 ##

<table width="100%">
	<tr>
		<th>VIM工作模式</th>
	</tr>
	<tr>
		<td class="center">
			<img src="./img/vim/vim_01.png" />
		</td>
	</tr>
</table>

## 命令行模式 ##
命令行模式可用的按键说明，光标移动、复制粘贴、查找替换等。

<table width="100%">
	<tr>
		<th colspan="2">移动光标的方法</th>
	</tr>
	<tr>
		<td>h或向左箭头(←)</td>
		<td>光标向左移动一个字符</td>
	</tr>
	<tr>
		<td>j或向下箭头(↓)</td>
		<td>光标向下移动一个字符</td>
	</tr>
	<tr>
		<td>k或向上箭头(↑)</td>
		<td>光标向上移动一个字符</td>
	</tr>
	<tr>
		<td>l或向右箭头(→)</td>
		<td>光标向右移动一个字符</td>
	</tr>
	<tr>
		<td colspan="2">如果你将右手放在键盘上的话，你会发现hjkl是排列在一起的，因此可以使用这四个按键来移动光标。如果想要进行多次移动的话，例如向下移动30行，可以使用“30j”或“30↓”的组合按键，即加上想要进行的次数后，按下操作即可</td>
	</tr>
	<tr class='red'>
		<td>[ctrl]+[f]</td>
		<td>屏幕向下移动一页，相当于(Page Down)</td>
	</tr>
	<tr class='red'>
		<td>[ctrl]+[b]</td>
		<td>屏幕向上移动一页，相当于(Page Up)</td>
	</tr>
	<tr>
		<td>[ctrl]+[d]</td>
		<td>屏幕向下移动半页</td>
	</tr>
	<tr>
		<td>[ctrl]+[u]</td>
		<td>屏幕向上移动半页</td>
	</tr>
	<tr>
		<td>+</td>
		<td>光标移动到非空格符的下一行</td>
	</tr>
	<tr>
		<td>-</td>
		<td>光标移动到非空格符的上一行</td>
	</tr>
	<tr>
		<td>n[space]</td>
		<td>n表示数字，例如20。按下数字后再按空格键，光标会向右移动这一行的n个字符。</td>
	</tr>
	<tr class="red">
		<td>0或功能键[Home]</td>
		<td>这是数字“0”，移动到这一行的最前面字符处</td>
	</tr>
	<tr class="red">
		<td>$或功能键[End]</td>
		<td>移动到这一行的最后面字符处</td>
	</tr>
	<tr>
		<td>H</td>
		<td>光标移动到这个屏幕的最上方那一行的第一个字符</td>
	</tr>
	<tr>
		<td>M</td>
		<td>光标移动到这个屏幕的中央那一行的第一个字符</td>
	</tr>
	<tr>
		<td>L</td>
		<td>光标移动到这个屏幕的最下方那一行的第一个字符</td>
	</tr>
	<tr class="red">
		<td>G</td>
		<td>移动到这个文件的最后一行</td>
	</tr>
	<tr class="red">
		<td>nG</td>
		<td>n为数字。移动到这个文件的第n行。</td>
	</tr>
	<tr class="red">
		<td>gg</td>
		<td>移动到这个文件的第一行，相当于1G。</td>
	</tr>
	<tr>
		<td>n[Enter]</td>
		<td>n为数字。光标向下移动n行。</td>
	</tr>
	<tr>
		<th colspan="2">查找和替换</th>
	</tr>
	<tr class="red">
		<td>/word</td>
		<td>向下寻找一个名称为word的字符串。</td>
	</tr>
	<tr>
		<td>?word</td>
		<td>向上寻找一个字符串名称为word的字符串。</td>
	</tr>
	<tr>
		<td>n</td>
		<td>重复前一个查找的操作。</td>
	</tr>
	<tr>
		<td>N</td>
		<td>与n刚好相反，为反向进行前一个查找操作。</td>
	</tr>
	<tr>
		<td colspan="2">使用/word配合n和N是非常有帮助的，可以让你重复地找到一些关键字。</td>
	</tr>
	<tr class="red">
		<td>:n1,n2s/word1/word2/g</td>
		<td>n1,n2为数字。在第n1和n2行之间寻找word1这个字符串，并将该字符串替换为word2。</td>
	</tr>
	<tr class="red">
		<td>:1,$s/word1/word2/g</td>
		<td>从第一行到最后一行查找word1字符串，并将该字符串替换为word2。</td>
	</tr>
	<tr class="red">
		<td>:1,$s/word1/word2/gc</td>
		<td>从第一行到最后一行查找word1字符串，并将该字符串替换为word2。且在替换前显示提示字符给用户确认是否需要替换。</td>
	</tr>
	<tr>
		<th colspan="2">删除、复制与粘贴</th>
	</tr>
	<tr class="red">
		<td>x，X</td>
		<td>在一行字当中，x为向后删除一个字符(相当于Del)，X为向前删除一个字符(相当于Backspace)</td>
	</tr>
	<tr>
		<td>nx</td>
		<td>n为数字，连续向后删除n个字符。</td>
	</tr>
	<tr class="red">
		<td>dd</td>
		<td>删除光标所在的那一整行</td>
	</tr>
	<tr class="red">
		<td>ndd</td>
		<td>n为数字，删除光标所在的向下n行。</td>
	</tr>
	<tr>
		<td>d1G</td>
		<td>删除光标所在到第一行的所有数据。</td>
	</tr>
	<tr>
		<td>dG</td>
		<td>删除从光标所在到最后一行的所有数据。</td>
	</tr>
	<tr>
		<td>d$</td>
		<td>删除光标所在处到该行的最后一个字符。</td>
	</tr>
	<tr>
		<td>d0</td>
		<td>数字0，删除从光标所在处到该行的最前面一个字符。</td>
	</tr>
	<tr class="red">
		<td>yy</td>
		<td>复制光标所在的那一行</td>
	</tr>
	<tr class="red">
		<td>nyy</td>
		<td>n为数字。复制光标所在的向下n行。</td>
	</tr>
	<tr>
		<td>y1G</td>
		<td>复制光标所在行到第一行的所有数据。</td>
	</tr>
	<tr>
		<td>yG</td>
		<td>复制光标所在行到最后一行的所有数据。</td>
	</tr>
	<tr>
		<td>y0</td>
		<td>复制光标所在的那个字符到该行行首的所有数据。</td>
	</tr>
	<tr>
		<td>y$</td>
		<td>复制光标所在的那个字符到该行行尾的所有数据。</td>
	</tr>
	<tr class="red">
		<td>p, P</td>
		<td>p为将已复制的数据在光标的下一行粘贴，P则为粘贴在光标的上一行。</td>
	</tr>
	<tr>
		<td>J</td>
		<td>将光标所在行与下一行的数据结合成同一行。</td>
	</tr>
	<tr>
		<td>c</td>
		<td>重复删除多个数据，例如向下删除10行，[10cj]</td>
	</tr>
	<tr>
		<td class="red">u</td>
		<td>复原前一个操作。</td>
	</tr>
	<tr>
		<td class="red">[Ctrl]+r</td>
		<td>重复上一个操作</td>
	</tr>
	<tr>
		<td colspan="2">这个u和[Ctrl]+r是很常用的命令。一个是复原，另一个则是重做一次，利用它们，可以让你的编辑得心应手。</td>
	</tr>
	<tr class="red">
		<td>.</td>
		<td>小数点。意思是：重复前一个操作。如果你想要重复删除、重复粘贴等操作，按下小数点“.”就好了。</td>
	</tr>
</table>

## 插入模式 ##
命令行模式切换到插入模式的可用的按钮说明。

<table width="100%">
	<tr>
		<th colspan="2">进入插入或替换的编辑模式</th>
	</tr>
	<tr class="red">
		<td>i, l</td>
		<td>进入插入模式：<br/>i为从目前光标所在处插入，l为在目前所在行的第一个非空格处开始插入。</td>
	</tr>
	<tr class="red">
		<td>a, A</td>
		<td>进入插入模式：<br/>a为从目前光标所在的下一个字符处开始插入，A为从光标所在行的最后一个字符处开始插入。</td>
	</tr>
	<tr class="red">
		<td>o, O</td>
		<td>进入插入模式：<br/>小写字母o为在目前光标所在的下一行处插入新的一行；大写O为在目前光标所在处的上一行插入新的一行。</td>
	</tr>
	<tr class="red">
		<td>r, R</td>
		<td>进入替换模式：<br/>r只会替换光标所在的那一个字符一次；R会一直替换光标所在的文字，直到按下[Esc]键为止。</td>
	</tr>
	<tr>
		<td colspan="2">上面这些按键中，在vi界面的左下角处会出现“——INSERT——”或“——REPLACE——”的字样。</td>
	</tr>
	<tr class="red">
		<td>[ESC]</td>
		<td>退出编辑模式，回到一般模式中。</td>
	</tr>
</table>

## 命令行模式 ##
一般模式切换到命令行模式的可用按钮说明。

<table width="100%">
	<tr>
		<th colspan="2">命令行的保存、离开等命令</th>
	</tr>
	<tr class="red">
		<td>:w</td>
		<td>将编辑的数据写入硬盘文件中</td>
	</tr>
	<tr>
		<td>:w!</td>
		<td>若文件属性为“只读”时，强制写入该文件。不过具体是否可以写入，还要看文件的权限。</td>
	</tr>
	<tr class="red">
		<td>:q</td>
		<td>离开vi</td>
	</tr>
	<tr>
		<td>:q!</td>
		<td>若曾修改过文件，又不想存储，使用“!”为强制退出，不保存文件。</td>
	</tr>
	<tr>
		<td colspan="2">在vi中，那个“!”经常具有强制的意思。</td>
	</tr>
	<tr class="red">
		<td>:wq</td>
		<td>保存后离开，若为“:wq!”则为强制保存后离开。</td>
	</tr>
	<tr>
		<td>ZZ</td>
		<td>这是大写的Z。若文件没有更动，则不保存离开，若文件已经被更新过，则保存后离开。</td>
	</tr>
	<tr>
		<td>:w [filename]</td>
		<td>新建一个文件</td>
	</tr>
	<tr>
		<td>:e [filename]</td>
		<td>将编辑的数据保存为另一个文件(类似文件另存为)</td>
	</tr>
	<tr>
		<td>:r [filename]</td>
		<td>在编辑的数据中，读入另一个文件的数据，即将“filename”这个文件内容加到光标所在行后面。</td>
	</tr>
	<tr>
		<td>:n1,n2 w [filename]</td>
		<td>将n1到n2的内容保存成filename这个文件</td>
	</tr>
	<tr>
		<td>:! command</td>
		<td>暂时离开vim到命令行模式下执行command的显示结果。</td>
	</tr>
	<tr>
		<th colspan="2">vim环境的更改</th>
	</tr>
	<tr class="red">
		<td>:set nu</td>
		<td>显示行号，设置之后，会在每一行的前缀显示该行的行数。</td>
	</tr>
	<tr>
		<td>:set nonu</td>
		<td>取消行号，与set nu相反</td>
	</tr>
</table>

## 一个VIM习题 ##

	1、找到系统中的/etc/man.config文件。
	2、在/tmp这个目录下新建一个test目录。
	3、进入这个test目录中。
	4、将man.config文件复制到test目录下。
	5、使用vim编辑器打开man.config文件。
	6、设置显示行数
	7、将光标移动到58行，向右移动40个字符，查看双引号内是什么目录？
	8、将光标移动到第一行，并且向下查找字符串“bzip2”这个字符串，请问它在第几行？
	9、光标移动到50行。接下来，将50到100行之间的“man”改为“MAN”，并且一个一个挑选是否需要修改？执行的命令是？可以看到，结果显示改变了几个“man”？
	10、修改后，后悔了，有哪些方法可以恢复？
	11、复制65至73行共九行的内容(含MANPATH_MAP)，并且复制粘贴到最后一行之后。
	12、21到42行，以“#”开头的批注数据不要了，如何删除？
	13、将这个文件另存为man.config.bak的文件名。
	14、光标移动到27行第一个字符，并且删除15个字符，结果出现的第一个字符是什么？
	15、在第一行新增一行，在该行输入“i am superman”。
	16、保存退出。

## 更多 ##
<http://www.cnblogs.com/web-lover/archive/2012/01/21/2615950.html>