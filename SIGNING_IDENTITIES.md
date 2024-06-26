<p align="center">
<img src="./assets/signing_identities.png" alt="Signing Identities" width="500"/>
</p>

# Signing Identities

Currently `/security` utilizes SSH identites for signing communications. Communications that are signed will be signed with keys that are located in this document.

## Current and Past Identities used by `/security`

| Active |     Type    | Start of Use | End of Use |  Public Key / Fingerprint | Intended Purpose |
|--------|-------------|--------------|------------|---------------------------|------------------|
|   Yes  | SSH Ed25519 |  2023-10-10  |    N/A     | `AAAAC3NzaC1lZDI1NTE5AAAAIJM9d83nOz3eDRsK63DcS35rBW0QVRdhwF+X6U/jnwdK` `SHA256:AW1+2f/I6nZMaqW0TfOMEPkhN2BeKus0NdfWPPmVOFA` | `slashsecurity` |

## Validating signed documents

To validate a signature that was generated by an SSH identity from above, place the raw text file and raw text file signature included with the communication in a folder, and run the following command by inserting the active key above in the command below:

```sh
ssh-keygen -Y verify -f <(echo "slashsecurity ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIJM9d83nOz3eDRsK63DcS35rBW0QVRdhwF+X6U/jnwdK") -n file -I slashsecurity -s advisory.txt.sig < advisory.txt
Good "file" signature for slashsecurity with ED25519 key SHA256:AW1+2f/I6nZMaqW0TfOMEPkhN2BeKus0NdfWPPmVOFA
```
