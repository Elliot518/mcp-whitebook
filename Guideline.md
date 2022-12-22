### 1. General Architecture Layers

- Ecosystem Adapter Layer(EAL)
  It is the outlet of the whole micro-component ecosystem. It contains various front end projects which connect the ecosystems both internal and outside.

- Business Products Layer(BPL)
  It is the layer which contains various products of micro-component.

- Components Supporting Layer(CSL)
  It is the layer which contains various components or generic microservices centers of micro-component.

- Infrastructure Foudation Layer(IFL)
  It is the foundation of micro-component just like the base of the house.

#####Each layer of architecture contains several blocks.
#####Blocks are logical combinations of products belong to the layer.

- Nomenclatures

| Name     | Description                                          |
| -------- | ---------------------------------------------------- |
| Service  | Small scale logically combined microservices units.  |
| Center   | Middle scale logically combined microservices units. |
| Platform | Large scale logically combined microservices units.  |

####Platform > Center > Service

&nbsp;

### 2. Products of Ecosystem Adapter Layer(EAL)

#### 1) EAL Block 1:

[Catalog](EAL/Catalog.md)

&nbsp;

### 3. Products of Business Products Layer(BPL)

#### 1) BPL Block 1:



&nbsp;

### 4. Products of Components Supporting Layer(CSL)

#### 1) CSL Block 1: Servcie Management Block(SMB)

| Repository Name | Description                               |
| --------------- | ----------------------------------------- |
| mcp-rsc         | Remote service center of micro-component. |

<hr>

#### 2) CSL Block 2: Message Management Block(MMB)

| Repository Name | Description                                      |
| --------------- | ------------------------------------------------ |
| mcp-mcc         | Message communication center of micro-component. |

<hr>

#### 3) CSL Block 3: 

<hr>

#### 4) CSL Block 4:

<hr>

#### 5) CSL Block 5: Massive Storage Block

> Definition: Massive data storage products block including fast centralized cache service, including RDBMS and NoSQL massive data storage and fast and high performance query. Solutions will include databases and tables sharding, big data storage(eg: hive, hbase, es, mongodb etc), including non-structured objects storage management(eg: files, images, audios, videos and other big objects), providing online preview and query APIs.

| Repository Name | Description                                          |
| --------------- | ---------------------------------------------------- |
| mcp-ccs | Centralized cache service of micro-component. |
| mcp-msp         | Massive storage platform of micro-component.          |
| mcp-osc        | Objects storage center of micro-component. |

<hr>

#### 6) CSL Block 6: Infrastructure Block

| Repository Name | Description                              |
| --------------- | ---------------------------------------- |
| mcp-sms         | Send message service of micro-component. |
| mcp-ms          | Mail service of micro-component.         |

<hr>

#### 7) CSL Block 7: Application Diagnostic Block

| Repository Name | Description                    |
| --------------- | ------------------------------ |
| mcp-lc          | Log center of micro-component. |

<hr>

### 8) CSL Block 8: Artificial Intelligence Block

| Repository Name | Description |
| --------------- | ----------- |

&nbsp;

### 5. Products of Infrastructure Foudation Layer(IFL)

#### 5-1) IFL Block 1:

&nbsp;

### 6. Blueprint Bird View Diagram

![MicroComponent Blueprint V2.0](BluePrintV2.png)
