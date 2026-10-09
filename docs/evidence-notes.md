# My Hyper-V lab evidence

My October 2023 CMPS-368 lab combined VMware Workstation, Windows Server 2019, Hyper-V, and Windows failover-cluster configuration. The original Word document identifies me as its creator and last editor. Its screenshots are dated October 6, 2023. I have kept the portfolio summary in first person while distinguishing my recorded results from the assignment requirements.

## Sources

| Portfolio asset | Original source |
|---|---|
| `assets/cluster-created.png` | `CMPS-368 Hyper V Cluster.docx`, embedded `image2.png` |
| `assets/domain-computers.png` | Same document, embedded `image4.png` |
| `assets/cluster-node-down.png` | Same document, embedded `image5.png` |
| `assets/cluster-node-quarantined.png` | Same document, embedded `image6.png` |
| `assets/nic-team-host01.png` | Same document, embedded `image11.png` |
| `assets/nic-team-host02.png` | Same document, embedded `image12.png` |
| `assets/nested-vms-running.jpg` | `HA Assignment(KyleFischer).mp4`, sampled frame around 2:10 |
| `assets/iscsi-not-connected.jpg` | Same recording, sampled frame around 8:30 |

The six PNGs were extracted without changes. The two JPEGs are full-frame extracts from the recording, without crops or added annotations. Video times are approximate: frames were sampled at 20-second intervals. Thirty sampled frames were visually reviewed, alongside all thirteen embedded Word images. The recording's audio was not transcribed, and the video was not reviewed continuously. No original lab was rerun.

## What the record supports

- The cluster-creation wizard reports completion with `vHost-01` and `vHost-02`, Node Majority quorum, and IP `192.168.80.50`.
- Active Directory lists the cluster computer object and both virtual hosts.
- NIC teaming captures show configured virtual adapters and their states.
- A Hyper-V Manager capture shows the nested VMs Running on the parent host.
- Later captures include an additional cluster node, a Down node, a Quarantined node, and disconnected iSCSI storage.

## What remains unverified

My selected evidence does not show an automatically recovered guest VM on a second cluster node, a clean final cluster-validation report, a working shared-storage connection, completed VLAN isolation, or a working container webhost. The cluster-creation result and later fault states reflect different stages of the exercise.

The original Word document begins with assignment requirements, including host isolation, fencing, shared storage, and guest recovery. Those instructions were treated as context, not as proof that I completed each task. An additional screenshot shows an attempted Force Quorum start while the cluster is Down; that attempt does not establish successful recovery and is not included as a recommended procedure.

No plaintext credentials were identified in the selected captures during visual review. This review does not establish that every file in the original coursework archive is safe to publish. Instructor material and the complete recording remain outside the portfolio package.
