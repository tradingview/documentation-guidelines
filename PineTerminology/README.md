# Terminology



### Table of Contents

- ["argument" vs "parameter"](#argument-vs-parameter)
- [ID](#id)
- [Pine Script™](#pine-script)
- ["realtime" vs "real time"](#realtime-vs-real-time)
- ["timeframe"](#timeframe)



### "argument" vs "parameter"
We use "parameter" to designate the name of the values a function accepts when referring to the function's signature, or to the function in general. 
When referring to values passed to a function when calling it, we use "argument":
- *Defining the type of function **parameters** in library function declarations is mandatory.*
- *A "simple int" **argument** is required for the length parameter in ``sma()``.*

### ID
When referring to pointers to plots, hlines, drawings or arrays, we use "ID" for singular and "IDs" for plural:
- *Both IDs used to identify the lines to be filled in ``fill()`` must be either plot IDs or hline IDs.*
- *Drawing IDs are time series; array IDs are not.*

### indicator
We only use *indicator* to refer to Pine scripts containing the [``indicator()``](https://www.tradingview.com/pine-script-reference/v5/#fun_indicator) declaration statement. When referring to any Pine script, we use [*script*](#timeframe).

### Pine Script™
We use "Pine Script™" to name our language whenever we can. Because this form is heavier than the simple "Pine" we often used before, this means we cannot use it as often in a paragraph. Try to arrange your phrasing so that you do not overuse "Pine Script™" in too many close instances.

### "realtime" vs "real time"
We use "realtime" when it is an adjective and "real time" when "time" is used as a noun:
- *A realtime bar*
- *Realtime calculations*
- *A script running in real time*

### "timeframe"
We use "timeframe" to name what has historically be called "interval", "resolution" or "time frame".
