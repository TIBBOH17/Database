# Transaction
- A sequence of multiple operations perfomed on a database.
- Served as a single logical unit of a work.

# Properties of Transaction
- **Atomicity**
    - All operations within a transaction complete successfully, or do not complete at all.
- **Consistency**
    - Any transaction leaves the database in a consistent state, regardless of the outcome of the transaction.
- **Isolation**
    - Each transaction has access to an isolated version of the database.
- **Durability**
    - Permanent changes are made by the successful execution of a transaction.
 
# States of Transaction
<div align="center">
    <img src="https://github.com/TIBBOH17/Database/assets/121493257/80b97b6b-b314-4856-819d-aa75b81c48fd", width=70%>
</div>

- **Active**
    - The first state during the execution of a transaction.
- **Partially Committed**
    - A change has been executed in this state, but the database has not yet committed the change on disk.
- **Committed**
    - All the transaction updates are permanently stored in the database.
- **Failed**
    - A transaction fails or has been aborted in the active state or partially committed state
- **Aborted**
    - If the error is not resolved in the failed state, then the transaction is aborted and a rollback operation is performed to bring database to the the last saved consistent state.
- **Terminated**
    - The last and final transaction state after a committed or failed state.
