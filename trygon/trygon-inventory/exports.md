# Exports

{% hint style="danger" %}
<pre class="language-lua" data-title="" data-full-width="false"><code class="lang-lua">exports['uz_TrygonInventory']:RemoveItem(<a data-footnote-ref href="#user-content-fn-1">source</a>, <a data-footnote-ref href="#user-content-fn-2">item</a>, <a data-footnote-ref href="#user-content-fn-3">amount</a>, <a data-footnote-ref href="#user-content-fn-4">Slot</a>)
</code></pre>
{% endhint %}

<details>

<summary><em>How is it used ?</em></summary>

{% code overflow="wrap" %}
```lua
exports['uz_TrygonInventory']:RemoveItem(1, 'coffee', 2)
exports['uz_TrygonInventory']:RemoveItem(7, 'phone', 1, 4)
```
{% endcode %}

source: 1 - item: coffee - amount: 1 - Slot: 4

</details>

***

{% hint style="success" %}
<pre class="language-lua" data-title="Server - AddItem" data-overflow="wrap"><code class="lang-lua">exports['uz_TrygonInventory']:AddItem(<a data-footnote-ref href="#user-content-fn-5">source</a>, <a data-footnote-ref href="#user-content-fn-6">item</a>, <a data-footnote-ref href="#user-content-fn-7">amount</a>, <a data-footnote-ref href="#user-content-fn-8">info</a>)
</code></pre>
{% endhint %}

<details>

<summary><em>How is it used ?</em></summary>

```lua
exports['uz_TrygonInventory']:AddItem(4, 'coffee')
exports['uz_TrygonInventory']:AddItem(1, 'coffee', 2)
exports['uz_TrygonInventory']:AddItem(24, 'phone', 4, {Metadata: '302-912'})
```

</details>

***

{% hint style="warning" %}
<pre class="language-lua" data-title="Server - setUseItem"><code class="lang-lua">exports['uz_TrygonInventory']:setUseItem(<a data-footnote-ref href="#user-content-fn-2">itemName</a>, <a data-footnote-ref href="#user-content-fn-9">setFunction</a>)
</code></pre>
{% endhint %}

<details>

<summary><em>How is it used ?</em></summary>



<pre class="language-lua" data-overflow="wrap"><code class="lang-lua"><strong>exports['uz_TrygonInventory']:setUseItem('coffee', function(item, source)
</strong>    if exports['uz_TrygonInventory']:RemoveItem(source, item.ItemData.Name, 1, item.Slot) then
    end
end)
</code></pre>

</details>

***

{% hint style="info" %}
{% code title="Server - LoadInventory" overflow="wrap" %}
```lua
exports['uz_TrygonInventory']:LoadInventory(source)
```
{% endcode %}
{% endhint %}

<details>

<summary><em>How is it used ?</em></summary>

<pre class="language-lua" data-overflow="wrap"><code class="lang-lua">local Inventory = exports['uz_TrygonInventory']:LoadInventory(<a data-footnote-ref href="#user-content-fn-1">source</a>)

local Item = Inventory[tonumber(Slot)]
</code></pre>

</details>

***

{% hint style="success" %}
{% code title="Server - SaveInventory" %}
```lua
exports['uz_TrygonInventory']:SaveInventory(Name)
```
{% endcode %}
{% endhint %}

<details>

<summary><em>How is it used ?</em></summary>

<pre class="language-lua" data-overflow="wrap"><code class="lang-lua">exports['uz_TrygonInventory']:SaveInventory(<a data-footnote-ref href="#user-content-fn-10">'Players'</a>)

exports['uz_TrygonInventory']:SaveInventory('Stash')

exports['uz_TrygonInventory']:SaveInventory('Vehicles')
</code></pre>

</details>



[^1]: Player ID

[^2]: Item Name

[^3]: Delete item amount

[^4]: It can be left blank as desired

[^5]: ```
    Player ID
    ```

[^6]: ```
    Item Name
    ```

[^7]: ```
    If left blank, it is assumed as 1
    ```

[^8]: ```
    It can be left blank as desired
    ```

[^9]: Function

[^10]: Players - Stash - Vehicles
