<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>حجز مواعيد - د. أحمد (طبيب مختص)</title>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap" rel="stylesheet">
<style>
    :root {
        --primary: #0d9488; /* أخضر مخضر طبي */
        --primary-dark: #0f766e;
        --secondary: #0f172a;
        --bg: #f1f5f9;
        --white: #ffffff;
        --danger: #ef4444;
        --success: #22c55e;
        --warning: #f59e0b;
    }
    * { box-sizing: border-box; font-family: 'Cairo', sans-serif; }
    body { background-color: var(--bg); color: var(--secondary); margin: 0; padding: 0; }

    /* Navigation */
    nav { background: var(--secondary); color: var(--white); padding: 1rem; display: flex; justify-content: space-between; align-items: center; position: sticky; top: 0; z-index: 1000; box-shadow: 0 4px 6px -1px rgba(0,0,0,0.1); flex-wrap: wrap; gap: 10px; }
    nav h1 { margin: 0; font-size: 1.3rem; color: var(--primary); display: flex; align-items: center; gap: 8px; }
    .nav-btns { display: flex; gap: 8px; flex-wrap: wrap; }
    .nav-btns button { background: transparent; border: 1px solid var(--primary); color: var(--primary); padding: 6px 14px; cursor: pointer; border-radius: 6px; transition: 0.3s; font-family: inherit; font-size: 0.9rem; font-weight: 600; }
    .nav-btns button:hover, .nav-btns button.active { background: var(--primary); color: var(--white); }

    /* Layout */
    .container { max-width: 900px; margin: 2rem auto; padding: 0 1rem; }
    .card { background: var(--white); padding: 2rem; border-radius: 12px; box-shadow: 0 4px 6px -1px rgba(0,0,0,0.05); margin-bottom: 2rem; border: 1px solid #e2e8f0; }
    .card h2, .card h3 { color: var(--secondary); margin-top: 0; border-bottom: 2px solid #f1f5f9; padding-bottom: 10px; }
    .hidden { display: none !important; }
    .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; }
    @media (max-width: 700px) { .grid-2 { grid-template-columns: 1fr; } .card { padding: 1.2rem; } }

    /* Forms */
    .form-group { margin-bottom: 1.25rem; }
    label { display: block; margin-bottom: 0.5rem; font-weight: 600; font-size: 0.95rem; color: var(--secondary); }
    input, select, textarea { width: 100%; padding: 12px; border: 1px solid #cbd5e1; border-radius: 8px; font-size: 1rem; font-family: inherit; background: #f8fafc; transition: 0.2s; }
    input:focus, select:focus { outline: none; border-color: var(--primary); background: #fff; box-shadow: 0 0 0 3px rgba(13,148,136,0.1); }
    .btn-main { background: var(--primary); color: var(--white); border: none; width: 100%; padding: 14px; font-size: 1.1rem; font-weight: bold; border-radius: 8px; cursor: pointer; transition: 0.3s; font-family: inherit; }
    .btn-main:hover { background: var(--primary-dark); }
    .btn-secondary { background: transparent; color: var(--secondary); border: 1px solid #cbd5e1; padding: 8px 16px; border-radius: 6px; cursor: pointer; font-family: inherit; font-size: 0.9rem; }
    .btn-sm { padding: 5px 10px; font-size: 0.85rem; }

    /* Time slots */
    .time-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(80px, 1fr)); gap: 10px; margin-top: 10px; }
    .time-slot { padding: 10px 5px; border: 1px solid #cbd5e1; text-align: center; border-radius: 8px; cursor: pointer; transition: 0.2s; background: #f8fafc; font-size: 0.95rem; font-weight: 600; }
    .time-slot:hover:not(.booked) { border-color: var(--primary); background: #ccfbf1; }
    .time-slot.selected { background: var(--primary); color: var(--white); border-color: var(--primary); }
    .time-slot.booked { background: #e2e8f0; color: #94a3b8; cursor: not-allowed; text-decoration: line-through; border-color: #cbd5e1; }
    .empty-slots { grid-column: 1/-1; text-align: center; color: #64748b; padding: 15px; background: #f1f5f9; border-radius: 8px; }

    /* Table */
    table { width: 100%; border-collapse: collapse; margin-top: 1rem; font-size: 0.9rem; }
    th, td { border: 1px solid #e2e8f0; padding: 12px; text-align: right; vertical-align: middle; }
    th { background: #f1f5f9; color: var(--secondary); font-weight: 700; }
    tbody tr:nth-child(even) { background: #f8fafc; }
    .status-badge { padding: 4px 10px; border-radius: 20px; font-size: 0.8rem; color: white; display: inline-block; white-space: nowrap; font-weight: 600; }
    .status-pending { background: var(--warning); }
    .status-confirmed { background: var(--success); }
    .status-completed { background: var(--primary); }
    .status-cancelled { background: var(--danger); }

    /* Stats */
    .stats-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(140px, 1fr)); gap: 15px; margin-bottom: 2rem; }
    .stat-card { background: var(--white); color: var(--secondary); padding: 15px; border-radius: 10px; text-align: center; border: 1px solid #e2e8f0; border-top: 4px solid var(--primary); }
    .stat-card span { display: block; font-size: 1.5rem; color: var(--primary); font-weight: bold; margin-bottom: 5px; }
    .stat-card small { font-size: 0.85rem; color: #64748b; }

    /* Toast */
    #toast { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); background: var(--secondary); color: white; padding: 1rem 2rem; border-radius: 30px; display: none; z-index: 2000; box-shadow: 0 4px 15px rgba(0,0,0,0.2); max-width: 90%; text-align: center; font-weight: 600; }
    #toast.success { background: var(--success); }
    #toast.error { background: var(--danger); }

    /* Extras */
    .filter-bar { display: flex; gap: 10px; flex-wrap: wrap; margin-bottom: 1rem; align-items: end; }
    .filter-bar > div { flex: 1; min-width: 140px; }
    .days-check { display: flex; flex-wrap: wrap; gap: 8px; }
    .days-check label { display: flex; align-items: center; gap: 5px; background: #f8fafc; padding: 6px 12px; border-radius: 20px; cursor: pointer; font-weight: normal; font-size: 0.9rem; border: 1px solid #cbd5e1; margin-bottom: 0; }
    .days-check input { width: auto; }
    .booking-item { background: #f8fafc; padding: 15px; border-radius: 10px; margin-bottom: 10px; border-right: 4px solid var(--primary); display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 10px; }
    .booking-item .info { flex: 1; }
    .booking-item small { color: #64748b; display: block; margin-top: 4px; }
    .service-item { display: flex; justify-content: space-between; align-items: center; padding: 12px; background: #f8fafc; border-radius: 8px; margin-bottom: 8px; gap: 10px; border: 1px solid #e2e8f0; }
    .booking-code { background: #fef3c7; color: #b45309; padding: 2px 8px; border-radius: 4px; font-weight: bold; font-family: monospace; font-size: 1.1rem; border: 1px solid #fcd34d; }
</style>
</head>
<body>

<nav>
    <h1>🩺 د. أحمد - طبيب مختص</h1>
    <div class="nav-btns">
        <button data-page="client-page" onclick="showPage('client-page')">حجز موعد</button>
        <button data-page="my-page" onclick="showPage('my-page')">حجوزاتي</button>
        <button data-page="admin" onclick="goAdmin()">لوحة الطبيب</button>
    </div>
</nav>

<div class="container">

    <!-- واجهة المريض -->
    <div id="client-page" class="page">
        <div class="card">
            <h2 style="text-align:center; color: var(--primary);">احجز موعدك الآن</h2>
            <p style="text-align:center; color:#64748b; margin-top:-10px;">نظام حجز ذكي يمنع تداخل المواعيد نهائياً</p>
            
            <div id="booking-confirm" class="hidden" style="margin-bottom:15px;"></div>

            <div class="form-group">
                <label>نوع الزيارة</label>
                <select id="client-service" onchange="renderTimeSlots()"></select>
            </div>
            <div class="form-group">
                <label>تاريخ الزيارة</label>
                <input type="date" id="client-date" onchange="renderTimeSlots()">
            </div>
            <div class="form-group">
                <label>المواعيد المتاحة</label>
                <div id="time-slots" class="time-grid"></div>
            </div>
            <div class="form-group">
                <label>الاسم الكامل للمريض</label>
                <input type="text" id="client-name" placeholder="الاسم واللقب">
            </div>
            <div class="form-group">
                <label>رقم الهاتف</label>
                <input type="tel" id="client-phone" placeholder="05xxxxxxxx / 06xxxxxxxx / 07xxxxxxxx">
            </div>
            <div class="form-group">
                <label>العمر (اختياري)</label>
                <input type="number" id="client-age" placeholder="مثال: 35">
            </div>
            <div class="form-group">
                <label>ملاحظات طبية (اختياري)</label>
                <textarea id="client-notes" placeholder="أعراض، أمراض مزمنة، حساسية..." rows="2"></textarea>
            </div>
            <button class="btn-main" onclick="confirmBooking()">تأكيد الحجز ✅</button>
        </div>
    </div>

    <!-- حجوزاتي -->
    <div id="my-page" class="page hidden">
        <div class="card">
            <h2>حجوزاتي</h2>
            <p style="color:#64748b;">أدخل رقم هاتفك لعرض وإدارة مواعيدك</p>
            <div class="form-group">
                <label>رقم الهاتف</label>
                <input type="tel" id="my-phone" placeholder="05xxxxxxxx" oninput="renderMyBookings()">
            </div>
            <div id="my-empty" style="text-align:center; color:#64748b; padding:20px;">أدخل رقم هاتفك للبحث</div>
            <div id="my-bookings-content" class="hidden">
                <div id="my-bookings-list"></div>
            </div>
        </div>
    </div>

    <!-- دخول الطبيب -->
    <div id="login-page" class="page hidden">
        <div class="card" style="max-width:400px; margin:auto;">
            <h2 style="text-align:center;">دخول الطبيب</h2>
            <p style="text-align:center; color:#64748b; font-size:0.9rem;">كلمة المرور الافتراضية: <b>1234</b></p>
            <div class="form-group">
                <label>كلمة المرور</label>
                <input type="password" id="admin-pass" placeholder="****" onkeypress="if(event.key==='Enter')adminLogin()">
            </div>
            <button class="btn-main" onclick="adminLogin()">دخول</button>
        </div>
    </div>

    <!-- لوحة التحكم -->
    <div id="admin-page" class="page hidden">
        <div style="display:flex; justify-content:space-between; align-items:center; margin-bottom:15px; flex-wrap:wrap; gap:10px;">
            <h2 style="margin:0;">لوحة تحكم الطبيب</h2>
            <button class="btn-secondary" onclick="logout()">تسجيل الخروج</button>
        </div>

        <div class="stats-grid">
            <div class="stat-card"><span id="stat-today">0</span><small>مرضى اليوم</small></div>
            <div class="stat-card"><span id="stat-upcoming">0</span><small>المواعيد القادمة</small></div>
            <div class="stat-card"><span id="stat-total">0</span><small>إجمالي الحجوزات</small></div>
            <div class="stat-card"><span id="stat-profit">0 دج</span><small>الأرباح المتوقعة</small></div>
        </div>

        <div class="card">
            <h3>سجل المرضى والمواعيد</h3>
            <div class="filter-bar">
                <div><label>التاريخ</label><input type="date" id="filter-date" onchange="renderAdminTable()"></div>
                <div>
                    <label>الحالة</label>
                    <select id="filter-status" onchange="renderAdminTable()">
                        <option value="">الكل</option>
                        <option value="pending">قيد الانتظار</option>
                        <option value="confirmed">مؤكد</option>
                        <option value="completed">مكتمل</option>
                        <option value="cancelled">ملغي</option>
                    </select>
                </div>
                <div><label>بحث</label><input type="text" id="filter-search" placeholder="اسم أو هاتف" oninput="renderAdminTable()"></div>
                <div><button class="btn-secondary" onclick="clearFilters()" style="width:100%;">مسح</button></div>
            </div>
            <div style="overflow-x:auto;">
                <table>
                    <thead>
                        <tr>
                            <th>المريض</th>
                            <th>الزيارة</th>
                            <th>الموعد</th>
                            <th>السعر</th>
                            <th>الحالة</th>
                            <th>إجراء</th>
                        </tr>
                    </thead>
                    <tbody id="admin-bookings-table"></tbody>
                </table>
            </div>
        </div>

        <div class="grid-2">
            <div class="card">
                <h3>أنواع الزيارات والأسعار</h3>
                <div id="services-list" style="margin-bottom:15px;"></div>
                <h4 style="margin-bottom:10px;">إضافة نوع زيارة</h4>
                <input type="text" id="srv-name" placeholder="مثال: كشف أول" style="margin-bottom:10px">
                <input type="number" id="srv-price" placeholder="السعر (دج)" min="0" style="margin-bottom:10px">
                <input type="number" id="srv-duration" placeholder="المدة (دقائق)" min="5" style="margin-bottom:10px">
                <button class="btn-main" onclick="addService()" style="padding:10px; font-size:1rem;">إضافة</button>
            </div>

            <div class="card">
                <h3>ساعات العمل</h3>
                <div class="form-group">
                    <label>وقت البدء</label>
                    <input type="time" id="work-start">
                </div>
                <div class="form-group">
                    <label>وقت الإغلاق</label>
                    <input type="time" id="work-end">
                </div>
                <div class="form-group">
                    <label>أيام الإغلاق الأسبوعية</label>
                    <div class="days-check">
                        <label><input type="checkbox" class="day-check" value="0"><span>الأحد</span></label>
                        <label><input type="checkbox" class="day-check" value="1"><span>الإثنين</span></label>
                        <label><input type="checkbox" class="day-check" value="2"><span>الثلاثاء</span></label>
                        <label><input type="checkbox" class="day-check" value="3"><span>الأربعاء</span></label>
                        <label><input type="checkbox" class="day-check" value="4"><span>الخميس</span></label>
                        <label><input type="checkbox" class="day-check" value="5"><span>الجمعة</span></label>
                        <label><input type="checkbox" class="day-check" value="6"><span>السبت</span></label>
                    </div>
                </div>
                <button class="btn-main" onclick="saveSettings()" style="padding:10px; font-size:1rem;">حفظ الإعدادات</button>
            </div>
        </div>
    </div>

</div>

<div id="toast"></div>

<script>
// ============================================================
// الإعدادات الأساسية
// ============================================================
const ADMIN_PASSWORD = '1234';
const CURRENCY = 'دج';
const STORAGE_KEY = 'doctor_specialist_v2';
const BUFFER_TIME = 5; // وقت راحة بين المرضى (بالدقائق) لمنع التداخل

const DEFAULT_SERVICES = [
    { id: 1, name: 'كشف أول', price: 1000, duration: 30 },
    { id: 2, name: 'استشارة متابعة', price: 500, duration: 15 },
    { id: 3, name: 'جلسة تنظيف / علاج', price: 1500, duration: 45 }
];

// جلب البيانات
function loadData() {
    const s = localStorage.getItem(STORAGE_KEY + '_services');
    const b = localStorage.getItem(STORAGE_KEY + '_bookings');
    const st = localStorage.getItem(STORAGE_KEY + '_settings');
    return {
        services: s ? JSON.parse(s) : DEFAULT_SERVICES,
        bookings: b ? JSON.parse(b) : [],
        settings: st ? JSON.parse(st) : { start: '08:30', end: '17:00', closedDays: [5] } // الجمعة مغلق
    };
}

const _loaded = loadData();
let services = _loaded.services;
let bookings = _loaded.bookings;
let settings = _loaded.settings;
let selectedTime = null;
let isAdmin = sessionStorage.getItem('isAdmin') === 'true';

function save() {
    localStorage.setItem(STORAGE_KEY + '_services', JSON.stringify(services));
    localStorage.setItem(STORAGE_KEY + '_bookings', JSON.stringify(bookings));
    localStorage.setItem(STORAGE_KEY + '_settings', JSON.stringify(settings));
}

// ============================================================
// أدوات مساعدة
// ============================================================
function showToast(msg, type = 'success') {
    const t = document.getElementById('toast');
    t.innerText = msg;
    t.className = type;
    t.style.display = 'block';
    clearTimeout(t._timer);
    t._timer = setTimeout(() => t.style.display = 'none', 3000);
}
function timeToMinutes(t) { const p = t.split(':'); return Number(p[0]) * 60 + Number(p[1]); }
function minutesToTime(m) { return String(Math.floor(m / 60)).padStart(2, '0') + ':' + String(m % 60).padStart(2, '0'); }
function todayStr() {
    const d = new Date();
    return d.getFullYear() + '-' + String(d.getMonth() + 1).padStart(2, '0') + '-' + String(d.getDate()).padStart(2, '0');
}
function fmtDate(s) {
    if (!s) return '';
    const d = new Date(s + 'T00:00:00');
    const days = ['الأحد', 'الإثنين', 'الثلاثاء', 'الأربعاء', 'الخميس', 'الجمعة', 'السبت'];
    return days[d.getDay()] + ' ' + s;
}
function normalizePhone(p) { return (p || '').replace(/[\s\-()]/g, ''); }
function generateCode() { return 'C-' + Math.floor(1000 + Math.random() * 9000); }

// ============================================================
// التنقل
// ============================================================
function showPage(id) {
    document.querySelectorAll('.page').forEach(p => p.classList.add('hidden'));
    document.getElementById(id).classList.remove('hidden');
    document.querySelectorAll('.nav-btns button').forEach(b => {
        const dp = b.getAttribute('data-page');
        b.classList.toggle('active', dp === id || (dp === 'admin' && (id === 'admin-page' || id === 'login-page')));
    });
    if (id === 'client-page') initClientPage();
    if (id === 'my-page') renderMyBookings();
    if (id === 'admin-page') renderAdmin();
    window.scrollTo(0, 0);
}
function goAdmin() { if (isAdmin) showPage('admin-page'); else showPage('login-page'); }
function logout() { isAdmin = false; sessionStorage.removeItem('isAdmin'); showPage('client-page'); showToast('تم تسجيل الخروج'); }

// ============================================================
// الخوارزمية الذكية لمنع التداخل (مع وقت الراحة)
// ============================================================
function getAvailableSlots(date, duration) {
    if (!date) return { slots: [], closed: false };
    const dow = new Date(date + 'T00:00:00').getDay();
    if (settings.closedDays.includes(dow)) return { slots: [], closed: true };

    const startMin = timeToMinutes(settings.start);
    const endMin = timeToMinutes(settings.end);
    if (startMin >= endMin) return { slots: [], closed: false };

    const dayBookings = bookings.filter(b => b.date === date && b.status !== 'cancelled');
    const slots = [];

    // نتحرك بفارق 15 دقيقة كبداية أولية
    for (let m = startMin; m + duration <= endMin; m += 15) {
        // نهاية الجلسة الحالية + وقت الراحة
        const slotEndWithBuffer = m + duration + BUFFER_TIME;
        
        let conflict = false;
        for (let b of dayBookings) {
            const srv = services.find(s => s.id == b.serviceId);
            const bDur = srv ? srv.duration : 20;
            const bStart = timeToMinutes(b.time);
            const bEndWithBuffer = bStart + bDur + BUFFER_TIME;
            
            // شرط تقاطع الأوقات: 
            // وقت البدء الجديد يجب أن يكون بعد نهاية الحجز القديم (مع الراحة)
            // ووقت النهاية الجديد (مع الراحة) يجب أن يكون قبل بداية الحجز القديم
            if ((m < bEndWithBuffer) && (slotEndWithBuffer > bStart)) {
                conflict = true;
                break;
            }
        }
        slots.push({ time: minutesToTime(m), isAvailable: !conflict });
    }
    return { slots, closed: false };
}

// ============================================================
// واجهة المريض
// ============================================================
function initClientPage() {
    const srvSel = document.getElementById('client-service');
    srvSel.innerHTML = services.map(s => 
        `<option value="${s.id}">${s.name} — ${s.price} ${CURRENCY} (${s.duration} د)</option>`
    ).join('');

    const dateInput = document.getElementById('client-date');
    dateInput.min = todayStr();
    if (!dateInput.value || dateInput.value < todayStr()) dateInput.value = todayStr();
    
    document.getElementById('booking-confirm').classList.add('hidden');
    selectedTime = null;
    renderTimeSlots();
}

function renderTimeSlots() {
    const grid = document.getElementById('time-slots');
    const date = document.getElementById('client-date').value;
    const srvId = document.getElementById('client-service').value;
    const srv = services.find(s => s.id == srvId);

    if (!date || !srv) { grid.innerHTML = '<div class="empty-slots">اختر التاريخ والزيارة أولًا</div>'; return; }
    
    const res = getAvailableSlots(date, srv.duration);
    selectedTime = null;

    if (res.closed) { grid.innerHTML = '<div class="empty-slots">🔒 العيادة مغلقة في هذا اليوم</div>'; return; }
    if (res.slots.length === 0) { grid.innerHTML = '<div class="empty-slots">لا توجد مواعيد متاحة</div>'; return; }

    grid.innerHTML = res.slots.map(slot => {
        if (slot.isAvailable) {
            return `<div class="time-slot" onclick="selectSlot(this, '${slot.time}')">${slot.time}</div>`;
        } else {
            return `<div class="time-slot booked">${slot.time}</div>`;
        }
    }).join('');
}

function selectSlot(el, time) {
    document.querySelectorAll('.time-slot').forEach(s => s.classList.remove('selected'));
    el.classList.add('selected');
    selectedTime = time;
}

function confirmBooking() {
    const name = document.getElementById('client-name').value.trim();
    const phone = document.getElementById('client-phone').value.trim();
    const age = document.getElementById('client-age').value;
    const notes = document.getElementById('client-notes').value.trim();
    const srvId = document.getElementById('client-service').value;
    const date = document.getElementById('client-date').value;

    if (name.length < 3) return showToast('الرجاء إدخال الاسم الكامل', 'error');
    const digits = phone.replace(/\D/g, '');
    if (digits.length < 8 || digits.length > 15) return showToast('رقم هاتف غير صحيح', 'error');
    if (!selectedTime) return showToast('الرجاء اختيار وقت متاح', 'error');

    const srv = services.find(s => s.id == srvId);
    
    // التحقق مجدداً من التوفر (منع التداخل في نفس اللحظة)
    const res = getAvailableSlots(date, srv.duration);
    const isSlotStillAvailable = res.slots.find(s => s.time === selectedTime && s.isAvailable);
    
    if (!isSlotStillAvailable) {
        showToast('عذراً، تم حجز هذا الموعد للتو. اختر موعداً آخر', 'error');
        renderTimeSlots();
        return;
    }

    const bookingCode = generateCode();

    const booking = {
        id: 'B' + Date.now(), 
        code: bookingCode,
        name, phone, age, notes,
        serviceId: srvId, serviceName: srv.name, price: srv.price,
        date, time: selectedTime, status: 'pending',
        createdAt: new Date().toISOString()
    };
    bookings.push(booking);
    save();

    const confirmBox = document.getElementById('booking-confirm');
    confirmBox.innerHTML = `
        <div style="background:#ecfdf5; border:1px solid #10b981; border-radius:10px; padding:20px; text-align:center; box-shadow: 0 4px 6px rgba(0,0,0,0.05);">
            <h3 style="margin:0 0 10px 0; color:#047857;">✅ تم تسجيل حجزك بنجاح</h3>
            <p style="margin:5px 0;">رمز الحجز الخاص بك: <span class="booking-code">${bookingCode}</span></p>
            <small>${srv.name} — ${fmtDate(date)} — الساعة ${selectedTime}</small><br>
            <small style="color:#64748b; display:block; margin-top:10px;">يرجى الحضور قبل الموعد بـ 10 دقائق وإظهار رمز الحجز.</small>
        </div>
    `;
    confirmBox.classList.remove('hidden');

    document.getElementById('client-name').value = '';
    document.getElementById('client-phone').value = '';
    document.getElementById('client-age').value = '';
    document.getElementById('client-notes').value = '';
    
    renderTimeSlots();
    showToast('تم الحجز بنجاح!');
}

// ============================================================
// حجوزاتي للمريض
// ============================================================
function renderMyBookings() {
    const phone = document.getElementById('my-phone').value.trim();
    const empty = document.getElementById('my-empty');
    const content = document.getElementById('my-bookings-content');
    const list = document.getElementById('my-bookings-list');

    if (phone.length < 6) {
        content.classList.add('hidden'); empty.classList.remove('hidden');
        empty.innerText = 'أدخل رقم هاتفك لعرض حجوزاتك'; return;
    }
    
    const norm = normalizePhone(phone);
    const my = bookings.filter(b => normalizePhone(b.phone) === norm)
        .sort((a, b) => (a.date + a.time).localeCompare(b.date + b.time));
        
    if (my.length === 0) {
        content.classList.add('hidden'); empty.classList.remove('hidden');
        empty.innerText = 'لا توجد حجوزات لهذا الرقم'; return;
    }
    
    empty.classList.add('hidden'); content.classList.remove('hidden');
    const labels = { pending: 'قيد الانتظار', confirmed: 'مؤكد', completed: 'مكتمل', cancelled: 'ملغي' };
    
    list.innerHTML = my.map(b => {
        const canCancel = b.status === 'pending' || b.status === 'confirmed';
        return `
        <div class="booking-item">
            <div class="info">
                <strong>${b.serviceName}</strong> | رمز: <span class="booking-code" style="font-size:0.9rem;">${b.code}</span>
                <small>📅 ${fmtDate(b.date)} — 🕐 ${b.time}</small>
                <small>الحالة: <span class="status-badge status-${b.status}">${labels[b.status]}</span></small>
            </div>
            ${canCancel ? `<button class="btn-secondary btn-sm" onclick="cancelMyBooking('${b.id}')" style="color:#ef4444; border-color:#ef4444;">إلغاء</button>` : ''}
        </div>`;
    }).join('');
}

function cancelMyBooking(id) {
    if (!confirm('هل أنت متأكد من إلغاء الموعد؟')) return;
    const b = bookings.find(x => x.id === id);
    if (b) { b.status = 'cancelled'; save(); showToast('تم إلغاء الحجز'); renderMyBookings(); }
}

// ============================================================
// لوحة الطبيب
// ============================================================
function adminLogin() {
    if (document.getElementById('admin-pass').value === ADMIN_PASSWORD) {
        isAdmin = true; sessionStorage.setItem('isAdmin', 'true');
        document.getElementById('admin-pass').value = '';
        showPage('admin-page'); showToast('مرحباً دكتور');
    } else showToast('كلمة المرور خاطئة', 'error');
}

function renderAdmin() {
    renderAdminStats(); renderAdminTable(); renderServicesList(); loadSettingsForm();
}

function renderAdminStats() {
    const today = todayStr();
    const todayCount = bookings.filter(b => b.date === today && b.status !== 'cancelled').length;
    const upcoming = bookings.filter(b => b.date >= today && b.status !== 'cancelled' && b.status !== 'completed').length;
    const profit = bookings.filter(b => b.status !== 'cancelled').reduce((s, b) => s + (Number(b.price) || 0), 0);
    
    document.getElementById('stat-today').innerText = todayCount;
    document.getElementById('stat-upcoming').innerText = upcoming;
    document.getElementById('stat-total').innerText = bookings.length;
    document.getElementById('stat-profit').innerText = profit + ' ' + CURRENCY;
}

function renderAdminTable() {
    const fDate = document.getElementById('filter-date').value;
    const fStatus = document.getElementById('filter-status').value;
    const fSearch = document.getElementById('filter-search').value.trim();

    let filtered = bookings.slice().sort((a, b) => (b.date + b.time).localeCompare(a.date + a.time));
    if (fDate) filtered = filtered.filter(b => b.date === fDate);
    if (fStatus) filtered = filtered.filter(b => b.status === fStatus);
    if (fSearch) filtered = filtered.filter(b => (b.name || '').includes(fSearch) || (b.phone || '').includes(fSearch));

    const tbody = document.getElementById('admin-bookings-table');
    if (filtered.length === 0) {
        tbody.innerHTML = '<tr><td colspan="6" style="text-align:center; color:#64748b; padding:20px;">لا توجد حجوزات مطابقة</td></tr>';
        return;
    }
    
    const labels = { pending: 'قيد الانتظار', confirmed: 'مؤكد', completed: 'مكتمل', cancelled: 'ملغي' };
    
    tbody.innerHTML = filtered.map(b => {
        const opts = Object.keys(labels).map(k => `<option value="${k}" ${b.status === k ? 'selected' : ''}>${labels[k]}</option>`).join('');
        const notesHtml = b.notes ? `<br><small style="color:#ef4444;">ملاحظة: ${b.notes}</small>` : '';
        const ageHtml = b.age ? ` (${b.age} سنة)` : '';
        
        return `
        <tr>
            <td>
                <strong>${b.name}</strong>${ageHtml}<br>
                <small>${b.phone}</small>${notesHtml}
            </td>
            <td>${b.serviceName}<br><span class="booking-code">${b.code}</span></td>
            <td>${b.date}<br><small>${b.time}</small></td>
            <td>${b.price} ${CURRENCY}</td>
            <td><select onchange="updateStatus('${b.id}', this.value)" style="padding:6px; font-size:0.85rem; border-radius:6px;">${opts}</select></td>
            <td><button class="btn-secondary btn-sm" onclick="deleteBooking('${b.id}')" style="color:#ef4444; border-color:#ef4444;">حذف</button></td>
        </tr>`;
    }).join('');
}

function updateStatus(id, status) {
    const b = bookings.find(x => x.id === id);
    if (b) { b.status = status; save(); renderAdminStats(); renderAdminTable(); showToast('تم تحديث الحالة'); }
}
function deleteBooking(id) {
    if (!confirm('حذف هذا الحجز نهائياً؟')) return;
    bookings = bookings.filter(b => b.id !== id); save(); renderAdmin(); showToast('تم الحذف');
}
function clearFilters() {
    document.getElementById('filter-date').value = '';
    document.getElementById('filter-status').value = '';
    document.getElementById('filter-search').value = '';
    renderAdminTable();
}

function renderServicesList() {
    document.getElementById('services-list').innerHTML = services.map(s => `
        <div class="service-item">
            <span><strong>${s.name}</strong><br><small style="color:#64748b;">${s.price} ${CURRENCY} — ${s.duration} دقيقة</small></span>
            <button class="btn-secondary btn-sm" onclick="deleteService(${s.id})" style="color:#ef4444; border-color:#ef4444;">حذف</button>
        </div>
    `).join('');
}
function addService() {
    const name = document.getElementById('srv-name').value.trim();
    const price = Number(document.getElementById('srv-price').value);
    const duration = Number(document.getElementById('srv-duration').value);
    if (!name) return showToast('أدخل اسم الزيارة', 'error');
    if (!price || price <= 0) return showToast('أدخل سعراً صحيحاً', 'error');
    if (!duration || duration < 5) return showToast('أدخل مدة صحيحة', 'error');
    
    services.push({ id: Date.now(), name, price, duration });
    save(); 
    document.getElementById('srv-name').value = ''; document.getElementById('srv-price').value = ''; document.getElementById('srv-duration').value = '';
    renderServicesList(); showToast('تمت الإضافة');
}
function deleteService(id) {
    if (!confirm('حذف هذه الزيارة؟')) return;
    services = services.filter(s => s.id !== id); save(); renderServicesList(); showToast('تم الحذف');
}

function loadSettingsForm() {
    document.getElementById('work-start').value = settings.start;
    document.getElementById('work-end').value = settings.end;
    document.querySelectorAll('.day-check').forEach(cb => cb.checked = settings.closedDays.includes(Number(cb.value)));
}
function saveSettings() {
    const start = document.getElementById('work-start').value;
    const end = document.getElementById('work-end').value;
    if (!start || !end) return showToast('حدد الأوقات', 'error');
    if (timeToMinutes(start) >= timeToMinutes(end)) return showToast('وقت البدء يجب أن يكون قبل الإغلاق', 'error');
    const closedDays = [];
    document.querySelectorAll('.day-check').forEach(cb => { if (cb.checked) closedDays.push(Number(cb.value)); });
    settings = { start, end, closedDays };
    save(); showToast('تم حفظ الإعدادات');
}

// التشغيل
document.addEventListener('DOMContentLoaded', () => {
    if (isAdmin) showPage('admin-page');
    else showPage('client-page');
});
</script>

</body>
</html>
