


#  Dental Clinic – Appointment Booking AI ChatBot

An intelligent appointment and patient management system built in **n8n**, designed for seamless clinic operations and patient engagement through **Telegram**. From booking and rescheduling to reminders and clinic Q&A, this automated workflow ensures reliability, accuracy, and human-like interaction — powered by AI orchestration and database synchronization.

![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/workflows/dental_appointment_booking_system_main.png)
---


## 🎥 Demo Recordings
To help you visualize the system in action, here are walkthrough recordings of each core feature. These demos showcase how users interact with the chatbot, how appointments are managed, and how notifications flow through the system — all powered by seamless automation and intelligent orchestration.

<a href="https://www.dropbox.com/scl/fi/qmwlcvwub9r7k93p18mcm/New-Booking.mp4?rlkey=lum859qkhsjczyoulkbzxzn29&st=4x91biqr&dl=0" target="_blank">🎥 Watch Demo – New Booking</a>

<a href="https://www.dropbox.com/scl/fi/9xm14ymqa4x19fhg5kuaf/Upcoming-Booking.mp4?rlkey=3a53xdgdjtw0qgrqudm5otkc7&st=c07nrke5&dl=0" target="_blank">🎥 Watch Demo – Upcoming Booking</a>

<a href="https://www.dropbox.com/scl/fi/ll7lbfy0afyqlfaduyxww/Reschedule-Booking.mp4?rlkey=qo7t30xlm8gam2ph3rv502tai&st=7a9qevks&dl=0" target="_blank">🎥 Watch Demo – Reschedule Booking</a>

<a href="https://www.dropbox.com/scl/fi/h8hpu2m05rtqxymxnmzb2/Cancel-Booking.mp4?rlkey=mhpw8kfjz0uzu6fkrr6e1l8gm&st=ymszqgrk&dl=0" target="_blank">🎥 Watch Demo – Cancel Booking</a>

<a href="https://www.dropbox.com/scl/fi/i6wanyztupjqjexecvb7l/FAQ.mp4?rlkey=1wjb4v4cm35hljjkh2iiwjpie&st=st3fegsr&dl=0" target="_blank">🎥 Watch Demo – Ask Question</a>


## 📸 Workflow Overview

<!-- Add your screenshots below -->

### User And Patient Tools
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/workflows/dental_appointment_booking_system_user_patient_tool.png)

### Appointment Tools
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/workflows/dental_appointment_booking_system_appointment_tool.png)

### 📅 Booking & Calendar Scheduling Tools
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/workflows/dental_appointment_booking_system_schedule_calendar_tool.png)

### 💬 Knowledge Base (RAG Agent)
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/workflows/dental_appointment_booking_system_knowledge_base_tool.png)
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/workflows/dental_appointment_booking_system_knowledge_base.png)

### 🔔 Doctor/Receptionist Notifications
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/workflows/dental_appointment_booking_system_receptionist_daily_reminder.png)
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/workflows/dental_appointment_booking_system_new_appointment_notification.png)


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
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/test%20cases/test_user_patient.png)

### 📅 New Booking
# 🎥 [Watch Demo]([https://your.video.hosting/faq_demo.mp4](https://www.dropbox.com/scl/fi/qmwlcvwub9r7k93p18mcm/New-Booking.mp4?rlkey=lum859qkhsjczyoulkbzxzn29&st=4x91biqr&dl=0))
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/test%20cases/test_new_booking.png)

### 🔁 Rescheduling
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/test%20cases/test_reschedule_booking.png)

### ❌ Cancel Appointment
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/test%20cases/test_cancel_booking.png)

### 🔍 My Upcoming Bookings
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/test%20cases/test_upcoming_booking.png)
### 💬 Knowledge Base Queries
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/test%20cases/test_knowledge_base.png)

### 🔔 Notification & Reminder System
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/test%20cases/test_reminder_notification.png)

### 🧪 Test Logic Workflow
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/test%20cases/test_logic_workflow.png)

###  User Experience
![Workflow Diagram](https://github.com/Orekidesu/n8n-workflow-project-lists/raw/main/Assets/Dental%20Clinic%20Appointment%20Booking%20AI%20ChatBot/test%20cases/test_ux.png)

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

