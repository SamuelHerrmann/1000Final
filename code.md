<p><a href="README.md">Home</a></p>
<h1 id="required-block-of-code">Required Block of Code</h1>
<pre><code class="lang-python"><span class="hljs-keyword">import</span> math
print(math.pi)
do_calc = True
<span class="hljs-keyword">while</span>(do_calc == True):
    <span class="hljs-keyword">while</span> (True):
        <span class="hljs-keyword">try</span>:
            print(<span class="hljs-string">"-----------------------"</span>)
            print(<span class="hljs-string">"Shape Volume Calculator"</span>)
            print(<span class="hljs-string">"-----------------------"</span>)
            print(<span class="hljs-string">"1. Calculate volume of a cone"</span>)
            print(<span class="hljs-string">"2. Calculate volume of a cube"</span>)
            print(<span class="hljs-string">"3. Calculate volume of a cylinder"</span>)
            shape = input(<span class="hljs-string">"Choose 1, 2, or 3:"</span>)
        except ValueError:
            print(<span class="hljs-string">"The input you typed was invalid. please type 1, 2, or 3 to make selection."</span>)
        <span class="hljs-keyword">else</span>:
            <span class="hljs-keyword">if</span> (shape == <span class="hljs-string">"1"</span> or shape == <span class="hljs-string">"2"</span> or shape == <span class="hljs-string">"3"</span>):
                <span class="hljs-keyword">break</span>
            <span class="hljs-keyword">else</span>:
                print(<span class="hljs-string">"The input you typed was invalid. please type 1, 2, or 3 to make selection."</span>)
    <span class="hljs-keyword">if</span> (shape == <span class="hljs-string">"1"</span> or shape == <span class="hljs-string">"3"</span>):
        <span class="hljs-keyword">while</span>(True):
            <span class="hljs-keyword">try</span>:
                r=<span class="hljs-keyword">float</span>(input(<span class="hljs-string">"Enter radius:"</span>))
            except ValueError:
                print(<span class="hljs-string">"The value you entered was invalid. Only type numbers please."</span>)
            <span class="hljs-keyword">else</span>:
                <span class="hljs-keyword">break</span>
    <span class="hljs-keyword">while</span> (True):
        <span class="hljs-keyword">try</span>:
            h=<span class="hljs-keyword">float</span>(input(<span class="hljs-string">"Enter height:"</span>))
        except ValueError:
            print(<span class="hljs-string">"The value you entered was invalid. Only type numbers please."</span>)
        <span class="hljs-keyword">else</span>:
            <span class="hljs-keyword">break</span>
    <span class="hljs-keyword">if</span> (shape == <span class="hljs-string">"1"</span>):
        volume = math.pi*r*r*(h/3)
        name = <span class="hljs-string">"cone"</span>
    <span class="hljs-keyword">if</span> (shape == <span class="hljs-string">"2"</span>):
        volume = h*h*h
        name = <span class="hljs-string">"cube"</span>
    <span class="hljs-keyword">if</span> (shape == <span class="hljs-string">"3"</span>):
        volume = math.pi*r*r*h
        name = <span class="hljs-string">"cylinder"</span>
    print(<span class="hljs-string">"Volume of the "</span> + name +<span class="hljs-string">" is"</span>,volume)
    <span class="hljs-keyword">while</span> (True):
        <span class="hljs-keyword">try</span>:
            another_calc = input(<span class="hljs-string">"Do you want to perform another calculation? (y/n):"</span>)
        except ValueError:
            print(<span class="hljs-string">"The value you entered was invalid. Only type y for yes and n for no please."</span>)
        <span class="hljs-keyword">else</span>:
            <span class="hljs-keyword">if</span> (another_calc == <span class="hljs-string">"y"</span> or another_calc == <span class="hljs-string">"n"</span>):
                <span class="hljs-keyword">break</span>
            <span class="hljs-keyword">else</span>:
                print(<span class="hljs-string">"The value you entered was invalid. Only type y for yes and n for no please."</span>)
    <span class="hljs-keyword">if</span> (another_calc != <span class="hljs-string">"y"</span>):
        do_calc = False
</code></pre>
