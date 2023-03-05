### 1. General Architecture Layers

- Ecosystem Adapter Layer(EAL)
  It is the outlet of the whole micro-component ecosystem. It contains various front end projects which connect the ecosystems both internal and outside.

- Business Products Layer(BPL)
  It is the layer which contains various products of micro-component.

- Components Supporting Layer(CSL)
  It is the layer which contains various components or generic microservices centers of micro-component.

- Infrastructure Foudation Layer(IFL)
  It is the foundation of micro-component just like the base of the house.

##### Each layer of architecture contains several blocks.
##### Blocks are logical combinations of products belong to the layer.

- Nomenclatures

| Name     | Description                                          |
| -------- | ---------------------------------------------------- |
| Service  | Small scale logically combined microservices units.<br>Containing just server side code.  |
| Center   | Middle scale logically combined microservices units.<br>Containing both server side and front end code. |
| Platform | Large scale logically combined microservices units.<br>Containing several server side and front end code.  |
| Warehouse | A bunch of code gathering together for developers to pick. |

#### Platform > Center > Service
#### Warehouse = Code Templates

&nbsp;

### 2. Main catalogs of blocks in four layers
#### 2-1. Ecosystem Adapter Layer(EAL)

| Block Name | Catalog Link         |
| -------- | -----------------------|
| B2C Business | [README](EAL/Block1/Catalog.md) |
| Intelligent Industry | [README](EAL/Block2/Catalog.md) |

<hr>

#### 2-2. Business Products Layer(BPL)

| Block Name | Catalog Link         |
| -------- | -----------------------|
| Enterprise Management Block | [README](BPL/Block1/Catalog.md) |
| Electronic Commerce Block | [README](BPL/Block2/Catalog.md) |
| Investment Block | [README](BPL/Block3/Catalog.md) |

<hr>

#### 2-3. Components Supporting Layer(CSL)

| Block Name | Catalog Link         |
| -------- | -----------------------|
| Service Management Block | [README](CSL/Block1/README.md) |
| Enterprise Components Block | [README](CSL/Block2/Catalog.md) |
| Security Block | [README](CSL/Block3/Catalog.md) |
| Artificial Intelligence Block | [README](CSL/Block4/Catalog.md) |
| Massive Storage Block | [README](CSL/Block5/Catalog.md) |
| Infrastructure Block | [README](CSL/Block6/Catalog.md) |
| Application Diagnostic Block | [README](CSL/Block7/Catalog.md) |
| Components Warehouse Block | [README](CSL/Block8/README.md) |

&nbsp;

### 3. A Bird View Blue Print of MicroComponent V2

![MicroComponent Blueprint V2.0](BluePrintV2.png)

&nbsp;

### 4. Zeus Data Center

- Aegis Data Warehouse
  >It is the warehouse where Zeus Data Center stores data.

&nbsp;

- Wind

&nbsp;

- Rain ([Readme](ZDC/Rain/README.md))
  >Data batch&stream processing

&nbsp;

- Thunder

&nbsp;

- Bolt

&nbsp;

![Zeus Data Center V1.0](ZeusDataCenterV1.png)


