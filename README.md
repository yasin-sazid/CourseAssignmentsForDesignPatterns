# Design Patterns in Java

A collection of Java implementations and applied assignments exploring reusable object-oriented designs. The projects connect familiar pattern structures to concrete problems: graphical composition, event notification, interchangeable algorithms, and coordinated client/server behavior.

## Pattern catalogue

| Pattern | Implementation | Application |
| --- | --- | --- |
| Composite | `DesignPatterns/src/Composite` | Compose shapes and flags through a shared shape interface |
| Observer | `DesignPatterns/src/Observer` | Notify account, email, and SMS observers of channel activity |
| Singleton | `DesignPatterns/src/Singleton` | Access a shared instance through a controlled construction interface |
| Strategy | `DesignPatterns/src/Strategy` | Select Bkash or Rocket payment behavior at runtime |
| Template Method | `DesignPatterns/src/TemplateMethod` | Share a tour-package workflow across economy, deluxe, and luxury variants |

## Applied assignments

- **Composite drawing:** `Assignment/CompositeAssignment` combines shape objects with UI event handlers.
- **Observer auction:** `ObserverAssignment`, `ObserverAssignment2`, and `ObserverAssignmentServer` separate bidder clients from server-side auction and bidder handlers.
- **Strategy conversion:** `Assignment/StrategyAssignment` selects CSV, JSON, or XML output through `IConvertionMethod`. Input and converted examples accompany the source; its `Library/` directory contains a JSON dependency.

## Explore and run

Use a JDK and open each module as an independent Java project. Set the module's `src` directory as its source root and run the corresponding `ClientClass` or `MainClass`. For the core payment strategy example:

```bash
javac -d /tmp/pattern-classes DesignPatterns/src/Strategy/*.java
java -cp /tmp/pattern-classes Strategy.ClientClass
```

For the auction assignment, start `ObserverAssignmentServer` before its client modules. Configure the conversion assignment with its supplied JSON JAR on the classpath and run from the module directory so file paths resolve correctly.

The collection demonstrates interface-driven design, composition, callback-based collaboration, and separation of invariant workflows from interchangeable behavior.
