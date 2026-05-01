<div align="center">
 <h1>DMP Integration Middleware API </h1>
 <p>Automated Legal Compliance Reporting for Property Owners</p>
</div>

---

## 🏢 Type 1: Commercial / Short-Stay (HBMS Route)

**Target:** Hotels, Commercial Serviced Apartments, Guesthouses.

**Destination Endpoint:** DMP Hotel Boarder Information System.

**Action:** Triggered automatically during the check-in process.

### `POST /api/v1/dmp/hbms/check-in`

**Description:** Pushes encrypted guest identity data and live media to the DMP Hotel Boarder database.

**Example Payload:**

```json
{
 "dmp_property_id": "DMP_HOTEL_GUL_042",
 "guest_info": {
   "full_name": "John Doe",
   "nationality": "Bangladeshi",
   "document_type": "NID",
   "document_number": "19951234567890",
   "dob": "1995-08-15",
   "profession": "Software Engineer"
 },
 "media": {
   "live_photo_b64": "base64_string",
   "document_scan_b64": "base64_string"
 }
}
