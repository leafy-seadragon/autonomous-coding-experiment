```python
_SCENT_PROFILES = {
    # Low complexity, well-documented, fresh
    ("low", "high", "fresh"): (
        "Fresh pine and morning dew",
        "This code is a joy to read — clean structure, well-documented, recently tended.",
        "🌲",
    ),
    # Low complexity, well-documented, stale
    ("low", "high", "stale"): (
        "Dusty library with pressed flowers",
        "Beautifully written but hasn't been touched in a while. Like finding a well-loved book in an attic.",
        "📚",
    ),
    # Low complexity, poor docs, fresh
    ("low", "low", "fresh"): (
        "Green banana and ozone",
        "Simple and recently written, but the lack of documentation makes it feel slightly unripe.",
        "🍌",
    ),
    # Low complexity, poor docs, stale
    ("low", "low", "stale"): (
        "Forgotten tupperware at the back of the fridge",
        "Simple but undocumented and untouched for ages. Nobody knows what it does anymore.",
        "🧊",
    ),
    # Medium complexity, well-documented, fresh
    ("medium", "high", "fresh"): (
        "Warm bread and fresh coffee",
        "Substantial but well-cared-for. The kind of code that feels nourishing to work with.",
        "☕",
    ),
    # Medium complexity, well-documented, stale
    ("medium", "high", "stale"): (
        "Aged cheese in a well-sealed cellar",
        "Complex but preserved well. The documentation is your guide through the aging process.",
        "🧀",
    ),
    # Medium complexity, poor docs, fresh
    ("medium", "low", "fresh"): (
        "Sweaty gym socks and energy drink",
        "Recently written with moderate complexity but zero hand-holding. Good luck, brave developer.",
        "🧦",
    ),
    # Medium complexity, poor docs, stale
    ("medium", "low", "stale"): (
        "Mildew and regret",
        "Medium complexity, undocumented, untouched. Every line is a mystery. You'll need a hazmat suit.",
        "😷",
    ),
    # High complexity, well-documented, fresh
    ("high", "high", "fresh"): (
        "Incense and polished mahogany",
        "Intricate and ambitious, but the documentation is your temple. Approach with reverence.",
        "🪵",
    ),
    # High complexity, well-documented, stale
    ("high", "high", "stale"): (
        "Old parchment and sealing wax",
        "A complex artifact preserved in documentation. Someone cared deeply about this once.",
        "📜",
    ),
    # High complexity, poor docs, fresh
    ("high", "low", "fresh"): (
        "Burning rubber and desperation",
        "Recently written, highly complex, and completely undocumented. Someone shipped this in a hurry.",
        "🔥",
    ),
    # High complexity, poor docs, stale
    ("high", "low", "stale"): (
        "Stale coffee and existential dread",
        "The legendary spaghetti. High complexity, no docs, untouched for ages. Abandon all hope, ye who enter here.",
        "💀",
    ),
}
```
