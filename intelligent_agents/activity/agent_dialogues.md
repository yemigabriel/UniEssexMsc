## Agent Communication Activity – KQML and KIF



This activity demonstrates the use of agent communication through KQML (Knowledge Query and Manipulation Language) and KIF (Knowledge Interchange Format). The interaction takes place between two agents: *Alice*, a procurement agent responsible for ordering stock, and *Bob*, a warehouse management agent responsible for tracking inventory.

Using KQML performatives like `ask-one` and `tell`, Alice and Bob exchange structured messages about the availability and specifications of 50-inch televisions. The content of each message is expressed in KIF, which allows for a formal, machine-readable representation of knowledge. For example, Alice asks for the stock level and HDMI slot count, and Bob responds with precise numerical values.

This dialogue illustrates how agent-based systems can support decentralised decision-making and autonomous interaction in a supply chain context. By separating communication semantics (via KQML) from knowledge representation (via KIF), the system enables agents to collaborate effectively even in distributed environments.


### Agent Dialogue (KQML and KIF)

#### Message 1: Alice → Bob (Query available stock)
```lisp
(KQML
  :performative ask-one
  :sender Alice
  :receiver Bob
  :language KIF
  :ontology warehouse-inventory
  :content
    (available-stock
      (item-type "50-inch-television")))
```

#### Message 2: Bob → Alice (Respond with stock level)
```lisp
(KQML
  :performative tell
  :sender Bob
  :receiver Alice
  :language KIF
  :ontology warehouse-inventory
  :content
    (stock-level
      (item-type "50-inch-television")
      (quantity 24)))
```

#### Message 3: Alice → Bob (Query HDMI slot details)
```lisp
(KQML
  :performative ask-one
  :sender Alice
  :receiver Bob
  :language KIF
  :ontology product-specs
  :content
    (hdmi-slot-count
      (item-type "50-inch-television")))
```

#### Message 4: Bob → Alice (Respond with HDMI slot count)
```lisp
(KQML
  :performative tell
  :sender Bob
  :receiver Alice
  :language KIF
  :ontology product-specs
  :content
    (hdmi-slot-count
      (item-type "50-inch-television")
      (count 3)))
```

---

### Agent Dialogue Table: Alice and Bob

| **Step** | **Sender → Receiver** | **KQML Performative** | **KIF Content (Summary)** |
|----------|-----------------------|------------------------|----------------------------|
| 1 | Alice → Bob | `ask-one` | What is the available stock of 50-inch televisions? |
| 2 | Bob → Alice | `tell` | There are 24 units of 50-inch televisions in stock. |
| 3 | Alice → Bob | `ask-one` | How many HDMI slots do the 50-inch televisions have? |
| 4 | Bob → Alice | `tell` | The 50-inch televisions have 3 HDMI slots. |

---