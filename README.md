# solana-batch-transfer
solana batch transfer &lt;max size 50 accounts transfer>



### 1. Install 

- ```
  download < sol_batch_transfer-1.0.1-py3-none- any.whl >
  ```

- ```
  pip install sol_batch_transfer-1.0.1-py3-none-any.whl
  ```

### 2. Usage

- ```
  from sol_batch_transfer.core import send_transaction
  
  if __name__ == '__main__':
      keypair_string = 'bs58 private key'
      receivers_list = ['receiver_01', 'receiver_01', ...]
      transfer_amount = 0.01
      tx_hash = send_transaction(bs58_string=keypair_string, receivers=receivers_list, amount=transfer_amount,endpoint="https://api.devnet.solana.com")
      print(tx_hash)
  ```

- ```
  1. default amount: 0.01
  2. default endpoint: https://api.devnet.solana.com
  ```
