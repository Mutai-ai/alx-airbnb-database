## INSERT 
-- Insert into Users
INSERT INTO users (user_id, first_name, last_name, email, password_hash, phone_number, role, created_at) VALUES
  ('11111111', 'Alice', 'Smith', 'alice@kim.com', 'alice_smith1', '1234567890', 'guest', 2025-05-13 14:42:59),
  ('22222222', 'Bob', 'Jones', 'bob@gmail.com', 'bobjones23', '2345678901', 'host', 2025-05-13 14:42:59),
  ('33333333', 'Carol', 'Lee', 'carol@hotmail.com', 'Carolee', '3456789012', 'admin', 2025-05-13 14:42:59
);

-- Insert into Locations
INSERT INTO locations (location_id, city, state, country) VALUES
  ('aaaaaaa1', 'New York', 'NY', 'USA'),
  ('aaaaaaa2', 'Los Angeles', 'CA', 'USA');

-- Insert into Properties
INSERT INTO properties (property_id, host_id, location_id, name, description, pricepernight, created_at, updated_at) VALUES
  ('bbbbbbb1', '223256', 'aaaaaaa1-aaa', 'Cozy Loft NYC', 'A small cozy loft in Manhattan.', 150.00, 2025-01-13 14:42:59, 2025-05-13 14:42:59);

-- Insert into Bookings
INSERT INTO bookings (booking_id, property_id, user_id, start_date, end_date, total_price, status, created_at) VALUES
  ('ccccccc1', 'bbbbbbb', '11r5r6', '2025-06-01', '2025-06-05', 600.00, 'confirmed', 2025-05-13 14:42:59);

-- Insert into Payments
INSERT INTO payments (payment_id, booking_id, amount, payment_method, payment_date) VALUES
  ('ddddddd1', 'ccccccc1', 600.00, 'credit_card', 2025-05-13 14:42:59);

-- Insert into Reviews
INSERT INTO reviews (review_id, property_id, user_id, rating, comment, created_at) VALUES
  ('eeeeeee1', 'bbbbbbb1-bbb', '115r5rg', 5, 'Amazing place to stay!', 2025-05-13 14:42:59);

-- Insert into Messages
INSERT INTO messages (message_id, sender_id, recipient_id, message_body, sent_at) VALUES
  ('fffffff1', '19967634', '222225', 'Hi, is your property available for early check-in?', 2025-05-13 14:42:59);
