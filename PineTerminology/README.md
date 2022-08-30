# Terminology



### Table of Contents

- ["argument" vs "parameter"](#argument-vs-parameter)
- [ID](#id)
- [indicator](#indicator)
- [library](#library)
- [Pine Script™](#pine-script)
- ["realtime" vs "real time"](#realtime-vs-real-time)
- [script](#script)
- [strategy](#strategy)
- [timeframe](#timeframe)



### "argument" vs "parameter"
We use *parameter* to designate the named placeholders defining the values that can be passed to a function when it is called in code. We use *argument* to name those values. A function signature thus has *parameters*, whereas a function call has *arguments*: 
- *Defining the type of function **parameters** in library function declarations is mandatory.*
- *A "simple int" **argument** is required for the length **parameter** in [``ta.sma()``](https://www.tradingview.com/pine-script-reference/v5/#fun_ta{dot}sma).*
- *The default value of the `shorttitle` **parameter** is the **argument** used for the `title` **parameter.***

### ID
When referring to pointers to plots, hlines, drawings or arrays, we use "ID" for singular and "IDs" for plural:
- *Both **IDs** used to identify the lines to be filled in ``fill()`` must be either plot **IDs** or hline IDs.*
- *Drawing **IDs** are time series.*

### indicator
We only use *indicator* to refer to Pine scripts containing the [``indicator()``](https://www.tradingview.com/pine-script-reference/v5/#fun_indicator) declaration statement. When referring to any Pine script, we use the generic term [*script*](#script).

### library
We only use *library* to refer to Pine scripts containing the [``library()``](https://www.tradingview.com/pine-script-reference/v5/#fun_library) declaration statement. When referring to any Pine script, we use the generic term [*script*](#script).

### Pine Script™
We use *Pine Script™* to name our language whenever we can. Because this form is heavier than the simple *Pine* we often used before, this means we cannot use it as often in a paragraph. Try to arrange your phrasing so that you do not overuse *Pine Script™* in too many close instances. We use *Pine script* to designate programs written in Pine Script™:
- *In **Pine Script™** v5, you can...*
- *The Community Scripts section of the website contains 100,000+ **Pine scripts**.*
- *On TradingView, indicators, strategies and libraries are written using our **Pine Script™** programming language.*

### "realtime" vs "real time"
We use *realtime* when it is an adjective and *real time* when *time* is used as a noun:
- *A **realtime** bar*
- ***Realtime** calculations*
- *A script running in **real time***

### script
We use *script* to designate Pine code that can be an [indicator](#indicator), a [strategy](#strategy) or a [library](#library).

### strategy
We only use *strategy* to refer to Pine scripts containing the [``strategy()``](https://www.tradingview.com/pine-script-reference/v5/#fun_strategy) declaration statement. When referring to any Pine script, we use the generic term [*script*](#script).

### timeframe
We use *timeframe* to name what has historically be called *interval*, *resolution* or *time frame*.
