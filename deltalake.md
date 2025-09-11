# 💾 Delta Lake

**Delta Lake** is an open-source **storage layer** on top of data lake that works seamlessly with **Apache Spark**.

---

## 🚀 Why Delta Lake?

Delta Lake enhances traditional data lakes by adding:

- ✅ **ACID Transactions** – Ensures data consistency even with concurrent reads/writes.
- 🔄 **Schema Enforcement & Evolution** – Prevents bad data and supports flexible schemas.
- 🕒 **Time Travel** – Query previous versions of your data for audits or debugging.
- ⚡ **Performance Optimizations** – Faster reads/writes with indexing and caching.

---

## 🔗 Delta Lake + Apache Spark

Delta Lake is built to work with **Apache Spark**. You use familiar Spark APIs to read, write, and transform data stored in Delta format.

### 🧪 Example: Reading and Writing Delta Tables

```python
# Read from a Delta table into a data frame
df = spark.read.format("delta").load("/mnt/delta/sales")

# Transform the data frame
df_filtered = df.filter(df["region"] == "Asia")

# Write back to a Delta table
df_filtered.write.format("delta").mode("overwrite").save("/mnt/delta/sales_asia")
```

---

---

## 📚 Other topics

**Change data feed(CDF)**
- similar to CDC (change data capture)
- tracks row level changes between version of a delta table
- read change events in batch with df.read and stream with df.readstream

SELECT * from tablechanges(<tablename>, versionstart, versionend)

**Universal Format(UniForm)**
- Delta Universal Format allows to read Delta tables with Iceberg and Hudi clients
- takes advantage of the fact that Delta Lake, Iceberg, and Hudi all consist of **Parquet** data files and a metadata layer
- A single copy of the data files provides access to clients of all formats.


---
## 📚 Learn More

Explore the official documentation:  
👉 [Delta Lake](https://www.youtube.com/watch?v=HQvAl0Bwpu8)
