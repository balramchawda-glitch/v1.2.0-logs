# ONDC Protocol Conformance Logs (nic2004:60232 - v1.2.0)

### Network Participant Information
- **Subscriber ID:** `ondc.onetab.ai`
- **Subscriber URL:** `https://ondc.onetab.ai/ondc-seller-v2`
- **Unique Key ID (ukId):** `cd7d4a95-6fbe-4d9a-aa6d-4fce634dd802`
- **Domain:** `nic2004:60232` (Logistics B2C)
- **Role:** `BAP` (Logistics Buyer Network Participant)
- **Protocol Workbench Session ID:** `7TDPzj_H5BrFLvZOhsUFmdx9zULtygaI`
- **Official Compliance Report ID:** `PW_7TDPzj_H5BrFLvZOhsUFmdx9zULtygaI`

---

## 1. Core Workflows (`ondc-logs/core/`)
Contains all mandatory core logistics order lifecycle logs:
- **Delivery Flow (`core/Delivery_flow/`)**: Transaction `19115b40-b849-4326-9a31-5aab5a42dc95` (14 steps: search, on_search, init, on_init, confirm, on_confirm, update, on_update, on_status, track, on_track).
- **Delivery Flow Without RTS (`core/Delivery_flow_without_rts/`)**: Transaction `45b3e5ed-e297-4564-91c2-5b346d5c73ef` (10 steps: search, on_search, init, on_init, confirm, on_confirm, on_status).
- **Buyer Cancel Flow (`core/Buyer_cancel_flow/`)**: Transaction `439adfe8-0c11-4f82-8621-6fd84517d046` (8 steps: search, on_search, init, on_init, confirm, on_confirm, cancel, on_cancel).
- **RTO Flow (`core/RTO_flow/`)**: Transaction `72e55c8d-f724-43aa-b420-04a0694cb2f5` (11 steps: search, on_search, init, on_init, confirm, on_confirm, on_status, on_cancel, on_status).

---

## 2. IGM Workflows (`ondc-logs/igm/`)
Contains the complete Issue and Grievance Management v1.0.0 lifecycle logs:
- **IGM Flow (`igm/IGM_flow/`)**: Transaction `cc813161-aa44-4ae6-bc91-9eee20c5c095` (18 steps: search through delivery, followed by `issue` (OPEN), `on_issue` (PROCESSING), `on_issue_status` (RESOLVED), and `issue` (CLOSED)).
