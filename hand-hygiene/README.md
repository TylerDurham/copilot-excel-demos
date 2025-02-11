# Hand Hygiene Tracking

# Key

> *Speakker notes*

**Additional considerations.**

~~~ copilot
Prompt
~~~

# Using XLOOKUP to "Join" Data

### Good

This prompt is good, as it exposes you to the *XLOOKUP* function. However, if I copy and paste the formula, it does not correctly name the actual table name and the actual key names.

``` copilot
I'd like to join data from the Hospital table with the Observation table. How can I do this?
```

### Better

This prompt gets you closer, because it uses the actual table name. However, it still (usually) misses the key names.

``` copilot
I'd like to join data from the DimHospital table with the Observation table. How can I do this?
```

### Best

Voila! Copilot hits on the table and key names, and should actually prompt you to insert the new column. No copy and paste needed.

``` copilot
Generate an xlookup in a new column called "hospital". Use the Observations hospital_id as the input, and search the id column of the DimHospital table.
```
