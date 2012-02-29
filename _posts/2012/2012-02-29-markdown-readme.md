---
layout: post
category : Misc
tags : [Markdown]
title: Markdown �﷨˵��
---
{% include JB/setup %}

**NOTE:** This is Simplelified  Chinese Edition Document of Markdown Syntax. If you are seeking for English Edition Document. Please refer to [Markdown: Syntax][eng-doc].

[eng-doc]:http://daringfireball.net/projects/markdown/syntax

**������** ����ĵ�����(fork)��[�������İ�](http://markdown.tw/)���ڴ˻����Ͻ����˷���ת���幤�������������ʵ�����ɫ�����ĵ��� Markdown �﷨��д������Ե�����[�鿴����Դ�ļ�][src1]�����������İ��ԭʼ�ļ�����[�鿴����][src] ����--By @[riku][t] / ����Ŀ�й��� [GitCafe][g]

**ע��** ����ĿͬʱҲ�й��� [Github][] �ϣ���ͨ�� fork��pull request ��ʽ����æ�Ľ�����Ŀ��

  [src1]: http://gitcafe.com/riku/Markdown-Syntax-CN/blob/master/syntax.md
  [src]: https://github.com/othree/markdown-syntax-zhtw/blob/master/syntax.md
  [t]: http://twitter.com/riku
  [g]: http://gitcafe.com/riku/Markdown-Syntax-CN
  [Github]: https://github.com/riku/Markdown-Syntax-CN

Markdown �﷨˵�� (�������İ�) / ([����鿴��������](./basic.html))
================

*   [����](#overview)
    *   [��ּ](#philosophy)
    *   [���� HTML](#html)
    *   [�����ַ��Զ�ת��](#autoescape)
*   [����Ԫ��](#block)
    *   [����ͻ���](#p)
    *   [����](#header)
    *   [��������](#blockquote)
    *   [�б�](#list)
    *   [��������](#precode)
    *   [�ָ���](#hr)
*   [����Ԫ��](#span)
    *   [����](#link)
    *   [ǿ��](#em)
    *   [����](#code)
    *   [ͼƬ](#img)
*   [����](#misc)
    *   [��б��](#backslash)
    *   [�Զ�����](#autolink)
*   [��л](#acknowledgement)

* * *

<h2 id="overview">����</h2>

<h3 id="philosophy">��ּ</h3>

Markdown ��Ŀ����ʵ�֡��׶���д����

�ɶ��ԣ�������Σ���������Ҫ�ġ�һ��ʹ�� Markdown ��ʽ׫д���ļ�Ӧ�ÿ���ֱ���Դ��ı����������ҿ�������������������ǩ���Ǹ�ʽָ�������ɡ�Markdown �﷨�ܵ�һЩ���� text-to-HTML ��ʽ��Ӱ�죬���� [Setext] [1]��[atx] [2]��[Textile] [3]��[reStructuredText] [4]��[Grutatext] [5] �� [EtText] [6]������������Դ��ʵ�Ǵ��ı������ʼ��ĸ�ʽ��

  [1]: http://docutils.sourceforge.net/mirror/setext.html
  [2]: http://www.aaronsw.com/2002/atx/
  [3]: http://textism.com/tools/textile/
  [4]: http://docutils.sourceforge.net/rst.html
  [5]: http://www.triptico.com/software/grutatxt.html
  [6]: http://ettext.taint.org/doc/

��֮�� Markdown ���﷨ȫ��һЩ��������ɣ���Щ���ž�������ϸѡ��������һĿ��Ȼ�����磺���������Լ����Ǻţ�����������\*ǿ��\*��Markdown ���б��������ţ������б�Markdown ���������ÿ������������������һ�����֣����������ڵ����ʼ��м�����������

<h3 id="html">���� HTML</h3>

Markdown �﷨��Ŀ���ǣ���Ϊһ�������������*��д*���ԡ�

Markdown ������Ҫȡ�� HTML������Ҳû��Ҫ��������������﷨������٣�ֻ��Ӧ HTML ��ǵ�һС���֡�Markdown �Ĺ���*����*Ҫʹ�� HTML �ĵ���������д�����ҿ����� HTML �Ѿ�������д�ˡ�Markdown �������ǣ������ĵ������׶���д������ġ�HTML ��һ��*����*�ĸ�ʽ��Markdown ��һ��*��д*�ĸ�ʽ����������Markdown �ĸ�ʽ�﷨ֻ���Ǵ��ı����Ժ��ǵķ�Χ��

���� Markdown ���Ƿ�Χ֮�ڵı�ǩ��������ֱ�����ĵ������� HTML ׫д������Ҫ�����ע���� HTML ���� Markdown��ֻҪֱ�Ӽӱ�ǩ�Ϳ����ˡ�

Ҫ��Լ��ֻ��һЩ HTML ����Ԫ�بD�D���� `<div>`��`<table>`��`<pre>`��`<p>` �ȱ�ǩ��������ǰ����Ͽ�����������������������Ҫ�����ǵĿ�ʼ��ǩ���β��ǩ�������Ʊ����ո���������Markdown �����������㹻���ܣ������� HTML �����ǩ����ϲ���Ҫ�� `<p>` ��ǩ��

�������£��� Markdown �ļ������һ�� HTML ���

    ����һ����ͨ���䡣

    <table>
        <tr>
            <td>Foo</td>
        </tr>
    </table>

    ������һ����ͨ���䡣

��ע�⣬�� HTML �����ǩ��� Markdown ��ʽ�﷨�����ᱻ�������磬���� HTML ������ʹ�� Markdown ��ʽ��`*ǿ��*`��û��Ч����

HTML �����Σ����ڣ���ǩ�� `<span>`��`<cite>`��`<del>` ������ Markdown �Ķ��䡢�б���Ǳ���������ʹ�á����ո���ϰ�ߣ��������Բ��� Markdown ��ʽ����ֱ�Ӳ��� HTML ��ǩ����ʽ��������˵��������Ƚ�ϲ�� HTML �� `<a>` �� `<img>` ��ǩ������ֱ��ʹ����Щ��ǩ�������� Markdown �ṩ�����ӻ���ͼ���ǩ�﷨��

�ʹ��� HTML �����ǩ�䲻ͬ��Markdown �﷨�� HTML ���α�ǩ������Ч�ġ�

<h3 id="autoescape">�����ַ��Զ�ת��</h3>

�� HTML �ļ��У��������ַ���Ҫ���⴦�� `<` �� `&` �� `<` ����������ʼ��ǩ��`&` ���������ڱ�� HTML ʵ�壬�����ֻ����Ҫ��ʾ��Щ�ַ���ԭ�ͣ������Ҫʹ��ʵ�����ʽ������ `&lt;` �� `&amp;`��

`&` �ַ������������ĵ���д������ĥ�������Ҫ��`AT&T`�� �������Ҫд�ɡ�`AT&amp;T`��������ַ�е� `&` �ַ�ҲҪת����������Ҫ���ӵ���

    http://images.google.com/images?num=30&q=larry+bird

�����Ҫ����ַת��дΪ��

    http://images.google.com/images?num=30&amp;q=larry+bird

���ܷŵ����ӱ�ǩ�� `href` ���������˵Ҳ֪��������׺��ԣ���Ҳ������ HTML ��׼��������鵽�Ĵ����У��������ġ�

Markdown ���������Ȼ����д�ַ�����Ҫת����������������ˡ������ʹ�õ� `&` �ַ��� HTML �ַ�ʵ���һ���֣����ᱣ��ԭ״���������ᱻת���� `&amp`;��

���������Ҫ���ĵ��в���һ����Ȩ���� `?`�����������д��

    &copy;

Markdown �ᱣ����������������д��

    AT&T

Markdown �ͻὫ��תΪ��

    AT&amp;T

���Ƶ�״��Ҳ�ᷢ���� `<` �����ϣ���Ϊ Markdown ���� [���� HTML](#html) ��������ǰ� `<` ������Ϊ HTML ��ǩ�Ķ����ʹ�ã��� Markdown Ҳ����������κ�ת�������������д��

    4 < 5

Markdown �������ת��Ϊ��

    4 &lt; 5

������Ҫע����ǣ�code ��Χ�ڣ����������ڻ������飬 `<` �� `&` �������Ŷ�*һ��*�ᱻת���� HTML ʵ�壬��������������Ժ����׵��� Markdown д HTML code ���� HTML ��Զ��ԣ� HTML �﷨�У���Ҫ�����е� `<` �� `&` ��ת��Ϊ HTML ʵ�壬������ HTML �ļ�����д�� HTML code����

* * *

<h2 id="block">����Ԫ��</h2>


<h3 id="p">����ͻ���</h3>

һ�� Markdown ��������һ�������������ı�����ɣ�����ǰ��Ҫ��һ�����ϵĿ��У����еĶ�������ʾ�Ͽ��������ǿյģ���ᱻ��Ϊ���С��ȷ�˵����ĳһ��ֻ�����ո���Ʊ���������Ҳ�ᱻ��Ϊ���У�����ͨ���䲻���ÿո���Ʊ����������

����һ�������������ı�����ɡ���仰��ʵ��ʾ�� Markdown ��������ڵ�ǿ�Ȼ��У����뻻�з�����������Ժ������󲿷ֵ� text-to-HTML ��ʽ��һ�������� Movable Type �ġ�Convert Line Breaks��ѡ��������ĸ�ʽ���ÿ�����з���ת�� `<br />` ��ǩ��

�����*ȷʵ*��Ҫ���� Markdown ������ `<br />` ��ǩ�Ļ����ڲ��봦�Ȱ����������ϵĿո�Ȼ��س���

��ȷ����Ҫ��ѵ��£���ӿո������� `<br />` �����Ǽ򵥵ء�ÿ�����ж�ת��Ϊ `<br />`���ķ����� Markdown �в����ʺϣ� Markdown �� email ʽ�� [��������][bq] �Ͷ����� [�б�][l] ��ʹ�û������Ű��ʱ�򣬲��������ã����������Ķ���

  [bq]: #blockquote
  [l]:  #list

<h3 id="header">����</h3>

Markdown ֧�����ֱ�����﷨���� [Setext] [1] ���� [atx] [2] ��ʽ��

�� Setext ��ʽ���õ��ߵ���ʽ������ `=` ����߽ױ��⣩�� `-` ���ڶ��ױ��⣩�����磺

    This is an H1
    =============

    This is an H2
    -------------

�κ������� `=` �� `-` ��������Ч����

�� Atx ��ʽ���������ײ��� 1 �� 6 �� `#` ����Ӧ������ 1 �� 6 �ף����磺

    # ���� H1

    ## ���� H2

    ###### ���� H6

�����ѡ���Եء��պϡ��� atx ��ʽ�ı��⣬�ⴿ��ֻ�������õģ����Ǿ��������������Ƚ����ʣ���Ϳ�������β���� `#`������β�� `#` ����Ҳ���úͿ�ͷһ�������׵ľ��ַ�������������Ľ�������

    # ���� H1 #

    ## ���� H2 ##

    ### ���� H3 ######


<h3 id="blockquote">�������� Blockquotes</h3>

Markdown �������������ʹ������ email ���� `>` �����÷�ʽ������㻹��Ϥ�� email �ż��е����Բ��֣����֪����ô�� Markdown �ļ��н���һ���������ã��ǻῴ�����������Լ��ȶϺ��У�Ȼ����ÿ�е���ǰ����� `>` ��

    > This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
    > consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
    > Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
    > 
    > Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
    > id sem consectetuer libero luctus adipiscing.

Markdown Ҳ������͵��ֻ����������ĵ�һ����ǰ����� `>` ��

    > This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
    consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
    Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

    > Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
    id sem consectetuer libero luctus adipiscing.

�������ÿ���Ƕ�ף����磺�����ڵ����ã���ֻҪ���ݲ�μ��ϲ�ͬ������ `>` ��

    > This is the first level of quoting.
    >
    > > This is nested blockquote.
    >
    > Back to the first level.

���õ�������Ҳ����ʹ�������� Markdown �﷨���������⡢�б���������ȣ�

	> ## ����һ�����⡣
	> 
	> 1.   ���ǵ�һ���б��
	> 2.   ���ǵڶ����б��
	> 
	> ����һЩ���Ӵ��룺
	> 
	>     return shell_exec("echo $input | $markdown_script");

�κ��������ı��༭���������ɵؽ��� email �͵����á������� BBEdit �У������ѡȡ���ֺ�Ȼ���ѡ����ѡ��*�������ýײ�*��

<h3 id="list">�б�</h3>

Markdown ֧�������б�������б�

�����б�ʹ���Ǻš��ӺŻ��Ǽ�����Ϊ�б��ǣ�

    *   Red
    *   Green
    *   Blue

��ͬ�ڣ�

    +   Red
    +   Green
    +   Blue

Ҳ��ͬ�ڣ�

    -   Red
    -   Green
    -   Blue

�����б���ʹ�����ֽ���һ��Ӣ�ľ�㣺

    1.  Bird
    2.  McHale
    3.  Parish

����Ҫ��һ���ǣ������б�����ʹ�õ����ֲ�����Ӱ������� HTML �����������б��������� HTML ���Ϊ��

    <ol>
    <li>Bird</li>
    <li>McHale</li>
    <li>Parish</li>
    </ol>

�������б���д�ɣ�

    1.  Bird
    1.  McHale
    1.  Parish

�������ǣ�

    3. Bird
    1. McHale
    8. Parish

�㶼��õ���ȫ��ͬ�� HTML ������ص����ڣ�������� Markdown �ļ����б����ֺ�����Ľ����ͬ����������һ�㣬�������ȫ�����������ֵ���ȷ�ԡ�

�����ʹ�������д���������һ����Ŀ��û��Ǵ� 1. ��ʼ����Ϊ Markdown δ�����ܻ�֧�������б�� start ���ԡ�

�б���Ŀ���ͨ���Ƿ�������ߣ�������ʵҲ������������� 3 ���ո���Ŀ��Ǻ�����һ��Ҫ��������һ���ո���Ʊ����

Ҫ���б�������Ư��������԰������ù̶�����������ã�

    *   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
        Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
        viverra nec, fringilla in, laoreet vitae, risus.
    *   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
        Suspendisse id sem consectetuer libero luctus adipiscing.

���������������Ҳ�У�

    *   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
    *   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing.

����б���Ŀ���ÿ��зֿ�������� HTML ʱ Markdown �ͻὫ��Ŀ������ `<p>` 
��ǩ��������������˵��

    *   Bird
    *   Magic

�ᱻת��Ϊ��

    <ul>
    <li>Bird</li>
    <li>Magic</li>
    </ul>

���������

    *   Bird

    *   Magic

�ᱻת��Ϊ��

    <ul>
    <li><p>Bird</p></li>
    <li><p>Magic</p></li>
    </ul>

�б���Ŀ���԰���������䣬ÿ����Ŀ�µĶ��䶼�������� 4 ���ո���� 1 ���Ʊ����

    1.  This is a list item with two paragraphs. Lorem ipsum dolor
        sit amet, consectetuer adipiscing elit. Aliquam hendrerit
        mi posuere lectus.

        Vestibulum enim wisi, viverra nec, fringilla in, laoreet
        vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
        sit amet velit.

    2.  Suspendisse id sem consectetuer libero luctus adipiscing.

�����ÿ�ж����������������ῴ�úܶ࣬��Ȼ���ٴεأ����������裬Markdown Ҳ����

    *   This is a list item with two paragraphs.

        This is the second paragraph in the list item. You're
    only required to indent the first line. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit.

    *   Another item in the same list.

���Ҫ���б���Ŀ�ڷŽ����ã��� `>` ����Ҫ������

    *   A list item with a blockquote:

        > This is a blockquote
        > inside a list item.

���Ҫ�Ŵ�������Ļ������������Ҫ����*����*��Ҳ���� 8 ���ո���� 2 ���Ʊ����

    *   һ�б������һ���б����飺

            <����д����>


��Ȼ����Ŀ�б�ܿ��ܻ᲻С�Ĳ�������������������д����

    1986. What a great season.

���仰˵��Ҳ���������׳���*����-���-�հ�*��Ҫ����������״����������ھ��ǰ����Ϸ�б�ܡ�

    1986\. What a great season.

<h3 id="precode">��������</h3>

�ͳ�����ص�д�����Ǳ�ǩ����ԭʼ��ͨ�������Ѿ��Ű�õĴ������飬ͨ����Щ�������ǲ���ϣ������һ������ļ��ķ�ʽȥ�Ű棬������ԭ����������ʾ��Markdown ���� `<pre>` �� `<code>` ��ǩ���Ѵ��������������

Ҫ�� Markdown �н�����������ܼ򵥣�ֻҪ�򵥵����� 4 ���ո���� 1 ���Ʊ���Ϳ��ԣ����磬��������룺

    ����һ����ͨ���䣺

        ����һ���������顣

Markdown ��ת���ɣ�

    <p>����һ����ͨ���䣺</p>

    <pre><code>����һ���������顣
    </code></pre>

���ÿ��һ�׵�������4 ���ո���� 1 ���Ʊ���������ᱻ�Ƴ������磺

    Here is an example of AppleScript:

        tell application "Foo"
            beep
        end tell

�ᱻת��Ϊ��

    <p>Here is an example of AppleScript:</p>

    <pre><code>tell application "Foo"
        beep
    end tell
    </code></pre>

һ�����������һֱ������û����������һ�У������ļ���β����

�ڴ����������棬 `&` �� `<` �� `>` ���Զ�ת�� HTML ʵ�壬�����ķ�ʽ����ǳ�����ʹ�� Markdown ���뷶���õ� HTML ԭʼ�룬ֻ��Ҫ�������ϣ��ټ��������Ϳ����ˣ�ʣ�µ� Markdown ������㴦�����磺

        <div class="footer">
            &copy; 2004 Foo Corporation
        </div>

�ᱻת��Ϊ��

    <pre><code>&lt;div class="footer"&gt;
        &amp;copy; 2004 Foo Corporation
    &lt;/div&gt;
    </code></pre>

���������У�һ��� Markdown �﷨���ᱻת���������Ǻű�ֻ���Ǻţ����ʾ����Ժ����׵��� Markdown �﷨׫д Markdown �﷨��ص��ļ���

<h3 id="hr">�ָ���</h3>

�������һ�������������ϵ��Ǻš����š�����������һ���ָ��ߣ����ڲ�����������������Ҳ�������ǺŻ��Ǽ����м����ո�����ÿ��д�������Խ����ָ��ߣ�

    * * *

    ***

    *****

    - - -

    ---------------------------------------


* * *

<h2 id="span">����Ԫ��</h2>

<h3 id="link">����</h3>

Markdown ֧��������ʽ�������﷨�� *����ʽ*��*�ο�ʽ*������ʽ��

��������һ�֣��������ֶ����� [������] ����ǡ�

Ҫ����һ��*����ʽ*�����ӣ�ֻҪ�ڷ������ź��������Բ���Ų�������ַ���Ӽ��ɣ�����㻹��Ҫ�������ӵ� title ���֣�ֻҪ����ַ���棬��˫���Ű� title ���ְ��������ɣ����磺

    This is [an example](http://example.com/ "Title") inline link.

    [This link](http://example.net/) has no title attribute.

�������

    <p>This is <a href="http://example.com/" title="Title">
    an example</a> inline link.</p>

    <p><a href="http://example.net/">This link</a> has no
    title attribute.</p>

�������Ҫ���ӵ�ͬ����������Դ�������ʹ�����·����

    See my [About](/about/) page for details.   

*�ο�ʽ*�����������������ֵ����ź����ٽ�����һ�������ţ����ڵڶ�������������Ҫ�������Ա�ʶ���ӵı�ǣ�

    This is [an example][id] reference-style link.

��Ҳ����ѡ���Ե��������������м����һ���ո�

    This is [an example] [id] reference-style link.

���ţ����ļ������⴦������԰������ǵ��������ݶ��������

    [id]: http://example.com/  "Optional Title Here"

�������ݶ������ʽΪ��

*   �����ţ�ǰ�����ѡ���Եؼ������������ո���������������������������
*   ����һ��ð��
*   ����һ�����ϵĿո���Ʊ��
*   �������ӵ���ַ
*   ѡ���Եؽ��� title ���ݣ������õ����š�˫���Ż�����������

�������������ӵĶ��嶼����ͬ��

	[foo]: http://example.com/  "Optional Title Here"
	[foo]: http://example.com/  'Optional Title Here'
	[foo]: http://example.com/  (Optional Title Here)

**��ע�⣺**��һ����֪�������� Markdown.pl 1.0.1 ����Ե����Ű����������� title��

������ַҲ�����÷����Ű�������

    [id]: <http://example.com/>  "Optional Title Here"

��Ҳ���԰� title ���Էŵ���һ�У�Ҳ���Լ�һЩ����������ַ̫���Ļ���������ȽϺÿ���

    [id]: http://example.com/longish/path/to/resource/here
        "Optional Title Here"

��ַ����ֻ���ڲ������ӵ�ʱ���õ���������ֱ�ӳ������ļ�֮�С�

���ӱ���ǩ��������ĸ�����֡��հ׺ͱ����ţ����ǲ�*��*���ִ�Сд�������������������һ���ģ�

	[link text][a]
	[link text][A]

*��ʽ���ӱ��*�����������ʡ��ָ�����ӱ�ǣ����������£����ӱ�ǻ���Ϊ��ͬ���������֣�Ҫ����ʽ���ӱ��ֻҪ���������ֺ������һ���յķ����ţ������Ҫ�� "Google" ���ӵ� google.com������Լ򻯳ɣ�

	[Google][]

Ȼ�����������ݣ�

	[Google]: http://google.com/

�����������ֿ��ܰ����հף��������ּ��͵ı����Ҳ�����������ʣ�

	Visit [Daring Fireball][] for more information.

Ȼ����Ŷ������ӣ�

	[Daring Fireball]: http://daringfireball.net/

���ӵĶ�����Է����ļ��е��κ�һ���ط����ұȽ�ƫ��ֱ�ӷ������ӳ��ֶ���ĺ��棬��Ҳ���԰��������ļ�����棬������ע��һ����

������һ���ο�ʽ���ӵķ�����

    I get 10 times more traffic from [Google] [1] than from
    [Yahoo] [2] or [MSN] [3].

      [1]: http://google.com/        "Google"
      [2]: http://search.yahoo.com/  "Yahoo Search"
      [3]: http://search.msn.com/    "MSN Search"

����ĳ����������Ƶķ�ʽд��

    I get 10 times more traffic from [Google][] than from
    [Yahoo][] or [MSN][].

      [google]: http://google.com/        "Google"
      [yahoo]:  http://search.yahoo.com/  "Yahoo Search"
      [msn]:    http://search.msn.com/    "MSN Search"

��������д�������������� HTML��

    <p>I get 10 times more traffic from <a href="http://google.com/"
    title="Google">Google</a> than from
    <a href="http://search.yahoo.com/" title="Yahoo Search">Yahoo</a>
    or <a href="http://search.msn.com/" title="MSN Search">MSN</a>.</p>

������������ʽд��ͬ��һ�����ݵ� Markdown �ļ����ṩ��Ϊ�Ƚ�֮�ã�

    I get 10 times more traffic from [Google](http://google.com/ "Google")
    than from [Yahoo](http://search.yahoo.com/ "Yahoo Search") or
    [MSN](http://search.msn.com/ "MSN Search").

�ο�ʽ��������ʵ�ص㲻�������ȽϺ�д���������ȽϺö����Ƚ�һ������ķ�����ʹ�òο�ʽ�����±���ֻ�� 81 ���ַ���������������ʽ��ȴ�����ӵ� 176 ����Ԫ��������ô� HTML ��ʽ��д������ 234 ����Ԫ���� HTML ��ʽ�У���ǩ���ı���Ҫ�ࡣ

ʹ�� Markdown �Ĳο�ʽ���ӣ��������ļ�������������������Ľ����������԰�һЩ�����ص�Ԫ�����Ƶ���������֮�⣬��Ϳ����������Ӷ��������µ��Ķ��о�����ϡ�

<h3 id="em">ǿ��</h3>

Markdown ʹ���Ǻţ�`*`���͵��ߣ�`_`����Ϊ���ǿ���ִʵķ��ţ��� `*` �� `_` ��Χ���ִʻᱻת���� `<em>` ��ǩ��Χ�������� `*` �� `_` �������Ļ�����ᱻת�� `<strong>`�����磺

    *single asterisks*

    _single underscores_

    **double asterisks**

    __double underscores__

��ת�ɣ�

    <em>single asterisks</em>

    <em>single underscores</em>

    <strong>double asterisks</strong>

    <strong>double underscores</strong>

������������ϲ������ʽ��Ψһ�������ǣ�����ʲô���ſ�����ǩ����Ҫ��ʲô���Ž�����

ǿ��Ҳ����ֱ�Ӳ��������м䣺

    un*frigging*believable

����**������ `*` �� `_` ���߶��пհ׵Ļ������Ǿ�ֻ�ᱻ������ͨ�ķ���**��

���Ҫ������ǰ��ֱ�Ӳ�����ͨ���ǺŻ���ߣ�������÷�б�ߣ�

    \*this text is surrounded by literal asterisks\*

<h3 id="code">����</h3>

���Ҫ���һС�����ڴ��룬������÷����Ű�����������`` ` ``�������磺

    Use the `printf()` function.

�������

    <p>Use the <code>printf()</code> function.</p>

���Ҫ�ڴ��������ڲ��뷴���ţ�������ö���������������ͽ����������Σ�

    ``There is a literal backtick (`) here.``

����﷨�������

    <p><code>There is a literal backtick (`) here.</code></p>

�������ε���ʼ�ͽ����˶����Է���һ���հף���ʼ�˺���һ����������ǰ��һ����������Ϳ��������ε�һ��ʼ�Ͳ��뷴���ţ�

	A single backtick in a code span: `` ` ``
	
	A backtick-delimited string in a code span: `` `foo` ``

�������

	<p>A single backtick in a code span: <code>`</code></p>
	
	<p>A backtick-delimited string in a code span: <code>`foo`</code></p>

�ڴ��������ڣ�`&` �ͷ�����**��**�ᱻ�Զ���ת�� HTML ʵ�壬��ʹ�ò��� HTML ԭʼ���ú����ף�Markdown ���������Σ�

    Please don't use any `<blink>` tags.

תΪ��

    <p>Please don't use any <code>&lt;blink&gt;</code> tags.</p>

��Ҳ��������д��

    `&#8212;` is the decimal-encoded equivalent of `&mdash;`.

�Բ�����

    <p><code>&amp;#8212;</code> is the decimal-encoded
    equivalent of <code>&amp;mdash;</code>.</p>



<h3 id="img">ͼƬ</h3>

�����Եأ�Ҫ�ڴ�����Ӧ�������һ������Ȼ�����﷨������ͼƬ����һ���Ѷȵġ�

Markdown ʹ��һ�ֺ����Ӻ����Ƶ��﷨�����ͼƬ��ͬ��Ҳ����������ʽ�� *����ʽ*��*�ο�ʽ*��

����ʽ��ͼƬ�﷨���������ǣ�

    ![Alt text](/path/to/img.jpg)

    ![Alt text](/path/to/img.jpg "Optional title")

��ϸ�������£�

*   һ����̾�� `!`
*   ����һ�������ţ��������ͼƬ���������
*   ����һ����ͨ���ţ��������ͼƬ����ַ����󻹿��������Ű�ס������
    ѡ���Ե� 'title' ���֡�

�ο�ʽ��ͼƬ�﷨�򳤵���������

    ![Alt text][id]

��id����ͼƬ�ο������ƣ�ͼƬ�ο��Ķ��巽ʽ�������ο�һ����

    [id]: url/to/image  "Optional title attribute"

��ĿǰΪֹ�� Markdown ��û�а취ָ��ͼƬ�Ŀ�ߣ��������Ҫ�Ļ��������ʹ����ͨ�� `<img>` ��ǩ��

* * *

<h2 id="misc">����</h2>

<h3 id="autolink">�Զ�����</h3>

Markdown ֧���ԱȽϼ�̵��Զ�������ʽ��������ַ�͵����ʼ����䣬ֻҪ���÷����Ű������� Markdown �ͻ��Զ�����ת�����ӡ�һ����ַ���������־ͺ����ӵ�ַһ�������磺

    <http://example.com/>

Markdown ��תΪ��

    <a href="http://example.com/">http://example.com/</a>

��ַ���Զ�����Ҳ�����ƣ�ֻ�� Markdown ������һ������ת���Ĺ��̣��������ַ�ת�� 16 ��λ��� HTML ʵ�壬�����ĸ�ʽ���Ժ�ŪһЩ���õ���ַ�ռ������ˣ����磺

    <address@example.com>

Markdown ��ת�ɣ�

    <a href="&#x6D;&#x61;i&#x6C;&#x74;&#x6F;:&#x61;&#x64;&#x64;&#x72;&#x65;
    &#115;&#115;&#64;&#101;&#120;&#x61;&#109;&#x70;&#x6C;e&#x2E;&#99;&#111;
    &#109;">&#x61;&#x64;&#x64;&#x72;&#x65;&#115;&#115;&#64;&#101;&#120;&#x61;
    &#109;&#x70;&#x6C;e&#x2E;&#99;&#111;&#109;</a>

����������棬����ִ�����ʵ�� `<a href="mailto:address@example.com">address@example.com</a>`������һ�����Ե���ġ�address@example.com�����ӡ�

������������Ȼ���Ժ�Ū���ٵĻ����ˣ���������ȫ���������������ܱ�ʲô��������Щ������������������������վ�����������ż��ġ���

<h3 id="backslash">��б��</h3>

Markdown �������÷�б��������һЩ���﷨������������ķ��ţ����磺�������Ҫ���Ǻż��������Աߵķ�ʽ������ǿ��Ч���������� `<em>` ��ǩ������������Ǻŵ�ǰ����Ϸ�б�ܣ�

    \*literal asterisks\*

Markdown ֧��������Щ����ǰ����Ϸ�б��������������ͨ�ķ��ţ�

    \   ��б��
    `   ������
    *   �Ǻ�
    _   ����
    {}  ������
    []  ������
    ()  ����
    #   ���ֺ�
    +   �Ӻ�
    -   ����
    .   Ӣ�ľ��
    !   ��̾��

<h2 id="acknowledgement">��л</h2>

��л [leafy7382][] Э�����룬[hlb][]��[Randylien][] ��æ��壬[ethantw][] ��[���ֱ�׼��ʽ?CSS Reset][]�� [WM][] �ر����ִ���

[leafy7382]:https://twitter.com/#!/leafy7382
[hlb]:http://iamhlb.com/
[Randylien]:http://twitter.com/randylien
[ethantw]:https://twitter.com/#!/ethantw
[���ֱ�׼��ʽ?CSS Reset]:http://ethantw.net/projects/han/
[WM]:http://kidwm.net/

��л [fenprace][]��[addv][]��

[fenprace]:https://github.com/fenprace
[addv]:https://github.com/addv