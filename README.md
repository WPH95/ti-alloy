## Ti-Alloy

### 钛合金， Tidb 扩展方案



Ti-alloy 基于了 tidb-plugin-framewok。为 tidb 增加大量用户定制化的功能扩展方案。

当前版本已完成

1. 和 mysql 接口相似的 UDF 定义，轻松为 tidb 添加 UDF

2. FDW (Foreign Data Wrapper) 原型完成 ，

   支持读/写操作

   参考 prometheus 的发展经历，实现了 Scan 和 SelectionScan 两种 Scan 接口





## Foreign Data Wrapper / Engine

1. base
   - [x] show engine
   - [x] show table status
   - [x] Explain
   - [x] Join tikv tale
2. Golang[low level]
   - [x] Insert
   - [x] Scan
   - [x] SelectionScan
   - [ ] optimization [TODO]
   - [ ] custom logic/physical Plan? [TODO]
   - [x] Create/Drop Table
3. Example:
   - [x] File[csv] Engine
   - [x] Elasticsearch Mock Engine
4. Python[high level][TODO]



### UDF

- [x] custom define function https://github.com/WPH95/tidb/pull/3>



### Third index support

- [ ] Fulltext
  - [ ] elasticsaeach


