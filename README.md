<h1>Resumos: Git</h1>
<br>
<h2>git reset</h2>
<h3>Para que serve?</h3>
<p>O comando <i>git reset</i> é utilizado para desfazer commits e alterações no repositório Git. Dependendo da opção usada (--soft, --mixed, --hard), ele pode afetar a posição do ponteiro HEAD, a área de stage (index) e o working directory (arquivos no diretório de trabalho).</p>
<h3>git reset --soft</h3>
<ul>
<li>
<p><strong>O que faz</strong>: A opção <i>--soft</i> defaz o commit, mas todas as mudanças associadas a esse commit são mantidas na aréa de stage.</p>
</li>
<li>
<p><strong>Como usar</strong>: Use <code>git reset --soft &lt;commit-anterior&gt;</code> ou então <code>git reset --soft HEAD~1</code> caso o commit que queira restaurar seja o mais recente.</p>
</li>
</ul>
<h3>git reset --mixed</h3>
<ul>
<li>
<p><strong>O que faz</strong>: A opção <i>--mixed</i> é a padrão, ou seja se executar <code>git reset &lt;commit-anterior&gt;</code> o reset agira como <i>--mixed</i>. Nessa função defaz o commit e as alterações voltam para unstaged.</p>
</li>
<li>
<p><strong>Como usar</strong>: Use <code>git reset --mixed &lt;commit-anterior&gt;</code>,<code>git reset --mixed HEAD~1</code> ou então apenas <code>git reset &lt;commit-anterior&gt;</code>.</p>
</li>
</ul>
</ul>
<h3>git reset --hard</h3>
<ul>
<li>
<p><strong>O que faz</strong>: A opção <i>--hard</i> defaz o commit e faz com que as alterações sejam desfeitas da area de trabalho, fazendo com que o arquivo fique conforme o commit que foi referenciado no <i>git reset --hard</i></p>
</li>
<li>
<p><strong>Como usar</strong>: Use <code>git reset --hard &lt;commit-anterior&gt;</code> ou então <code>git reset --hard HEAD~1</code> caso o commit que queira restaurar seja o mais recente.</p>
</li>
</ul>