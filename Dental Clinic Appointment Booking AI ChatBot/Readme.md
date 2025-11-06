


#  Dental Clinic – Appointment Booking AI ChatBot

An intelligent appointment and patient management system built in **n8n**, designed for seamless clinic operations and patient engagement through **Telegram**. From booking and rescheduling to reminders and clinic Q&A, this automated workflow ensures reliability, accuracy, and human-like interaction — powered by AI orchestration and database synchronization.

![Workflow Diagram](../Assets/BrightSmile/overview.png?raw=true "Clinic Workflow Overview")

---

## 📸 Workflow Overview

<!-- Add your screenshots below -->

### 🏁 Telegram Entry & Main Menu

![Workflow Diagram](../Assets/BrightSmile/1.png?raw=true "Telegram Entry")

### 🧍 User Verification & Patient Setup

![Workflow Diagram](../Assets/BrightSmile/2.png?raw=true "User and Patient Flow")

### 📅 Booking & Calendar Scheduling

![Workflow Diagram](../Assets/BrightSmile/3.png?raw=true "Booking Flow")

### 🔁 Rescheduling & Cancellations

![Workflow Diagram](../Assets/BrightSmile/4.png?raw=true "Rescheduling Flow")

### 🔍 My Upcoming Bookings & Reminders

![Workflow Diagram](../Assets/BrightSmile/5.png?raw=true "Upcoming Bookings")

### 💬 Knowledge Base (RAG Agent)

![Workflow Diagram](../Assets/BrightSmile/6.png?raw=true "RAG Agent Responses")

### 🔔 Doctor & Receptionist Notifications

![Workflow Diagram](../Assets/BrightSmile/7.png?raw=true "Notification System")

---

## 🔄 How It Works

1. **💬 Telegram Conversation Start**
   Users interact naturally through Telegram. Upon greeting, the assistant presents options — *New Booking, My Upcoming Bookings, Reschedule Booking,* or *Cancel Booking.*

2. **👤 User Verification**
   The assistant determines if the user already exists. Returning users are recognized instantly, while new users are guided through registration and patient setup.

3. **📋 Patient Selection & Data Handling**
   Users can select existing patients or add new ones. Records remain synced across all sessions.

4. **📆 Booking & Scheduling**
   Available clinic days and hours are presented automatically, excluding same-day or fully booked slots.

5. **✅ Appointment Confirmation**
   Once confirmed, the appointment is logged in the database and synchronized with the clinic’s master schedule.

6. **🔁 Rescheduling Flow**
   Users can move appointments at least one day in advance. The system updates both records and schedules instantly.

7. **❌ Cancellations**
   Appointments can be cancelled anytime. Both users and clinic staff receive real-time updates.

8. **📅 My Upcoming Bookings**
   Users can view grouped upcoming appointments with full details.

9. **💡 Knowledge Base Queries (RAG Agent)**
   For general inquiries—services, pricing, aftercare, or clinic policies—the AI retrieves verified information from the Bright Smile Dental Clinic Knowledge Base.

10. **🔔 Daily & Instant Notifications**

    * **Clinic Staff (Doctor/Receptionist):**

      * Immediate alerts for new, rescheduled, or cancelled appointments.
      * 7:00 AM daily summary of the day’s appointments.
    * **Patients:**

      * 7:00 AM appointment reminders on the day of their visit.

11. **⚙️ Seamless Orchestration**
    Every component—from chat flow to scheduling and reminders—is orchestrated to run in sequence, ensuring smooth automation without manual supervision.

---

## 🧩 Feature Testing Documentation

### 🧍 User & Patient Management

![Workflow Diagram](../Assets/BrightSmile/test_user_patient.png?raw=true "User & Patient Management Test")

### 📅 New Booking

![Workflow Diagram](../Assets/BrightSmile/test_booking.png?raw=true "Booking Test")

### 🔁 Rescheduling

![Workflow Diagram](../Assets/BrightSmile/test_reschedule.png?raw=true "Reschedule Test")

### ❌ Cancel Appointment

![Workflow Diagram](../Assets/BrightSmile/test_cancel.png?raw=true "Cancel Test")

### 🔍 My Upcoming Bookings

![Workflow Diagram](../Assets/BrightSmile/test_upcoming.png?raw=true "Upcoming Booking Test")

### 💬 Knowledge Base Queries

![Workflow Diagram](../Assets/BrightSmile/test_rag.png?raw=true "RAG Query Test")

### 🔔 Notification & Reminder System

![Workflow Diagram](../Assets/BrightSmile/test_reminders.png?raw=true "Reminders & Alerts Test")

---

## 🧪 Test Case Coverage

| Category          | Key Tests                                | Focus                             |
| ----------------- | ---------------------------------------- | --------------------------------- |
| 🧍 User Flow      | New/Returning user, multiple patients    | Account recognition & data recall |
| 📅 Booking        | Date validation, slot filtering          | Schedule reliability              |
| 🔁 Reschedule     | One-day restriction, resync check        | Logical accuracy                  |
| ❌ Cancel          | Real-time removal, graceful abort        | Calendar integrity                |
| 🔍 Upcoming       | Grouped output, readable formatting      | Data presentation                 |
| 💬 Knowledge Base | Service info, pricing, aftercare         | Retrieval accuracy                |
| 🔔 Reminders      | Doctor, receptionist, and patient alerts | Timely notifications              |
| 💾 Integration    | Calendar ↔ Database match                | Synchronization flow              |

---

## 🛠️ Tech Stack

* **n8n** – Workflow orchestration
* **Telegram Bot API** – Chat interface
* **Supabase** – Data and record storage
* **Calendar Integration** – Central scheduling
* **RAG Agent** – Intelligent knowledge retrieval
* **Scheduler System** – Automated daily reminders

---

## 🎯 Use Cases

### 🏥 Clinic Operations

* Automated patient scheduling and tracking
* Daily summaries for staff
* Minimal manual coordination between teams

### 💬 Patient Experience

* Simple, chat-based appointment system
* Friendly booking, rescheduling, and reminders
* Consistent updates and clear confirmations

### 🧠 Informational Queries

* Real-time answers about services, prices, and dental care
* Quick, human-like chatbot interactions powered by verified knowledge

---

### 🌐 Industry Adaptations

This workflow’s modular design can be applied to other service-based industries with slight adjustments to data structure and conversation flow:

| Industry                          | Adaptation Example                                                            |
| --------------------------------- | ----------------------------------------------------------------------------- |
| 🏨 **Spa & Wellness Centers**     | Replace “patients” with “clients” and add package or therapist selection.     |
| 💇 **Salon & Barbershops**        | Schedule hair, nail, or makeup appointments with stylist selection.           |
| 🐾 **Veterinary Clinics**         | Manage pet profiles, vaccination reminders, and check-up bookings.            |
| 🧘 **Fitness & Yoga Studios**     | Schedule classes, track attendance, and send instructor notifications.        |
| 📸 **Photography Studios**        | Book photo sessions, reschedule shoots, and send shoot-day reminders.         |
| 🚗 **Auto Service Centers**       | Manage car service bookings, maintenance reminders, and technician schedules. |
| 🧑‍⚕️ **General Medical Clinics** | Similar flow but multi-doctor assignment and insurance validation.            |

These industries can reuse the same booking → schedule → notification orchestration with only minimal field and message customization.

---

## 📌 Notes

* Fully automated with minimal supervision required
* Every user flow tested for valid and invalid inputs
* Daily notifications at **7:00 AM** for both staff and patients
* Scalable structure ready for online payments and insurance integration
* Modular design ensures each process (Booking → Calendar → Reminder) operates independently and reliably

---

